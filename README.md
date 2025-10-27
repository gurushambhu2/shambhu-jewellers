# Frontend — Jewelry Store (Vite + React)

## Quick start
1. `cd frontend`
2. `npm install`
3. `npm run dev`

Environment:
- Create `.env` file with `VITE_API_BASE` if your backend isn't on localhost:5000.
- For Razorpay include the script in index.html (already present).

## Direct Cloudinary uploads
This project uses a signed direct upload flow:
1. Frontend calls POST /api/cloudinary/sign to get signature, timestamp, api_key, and cloud_name.
2. Frontend uploads directly to Cloudinary using those values. Files do not pass through your backend.
