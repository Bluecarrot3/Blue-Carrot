# /media — Blue Carrot Upload Folder

This folder is where uploaded project media files will be saved once you add a backend.

## Supported File Types

| Type   | Extensions              | Color Tag |
|--------|-------------------------|-----------|
| Video  | `.mp4`, `.mov`, `.webm` | 🔵 Blue   |
| Audio  | `.mp3`, `.wav`, `.ogg`  | 🟣 Purple |
| Image  | `.png`, `.jpg`, `.gif`  | 🟢 Green  |
| PDF    | `.pdf`                  | 🔴 Red    |

## Max File Size
100 MB per file.

## How It Works (Current)
Right now the upload feature runs **in the browser only** — files are selected and previewed 
but not saved to a server. This is fine for a frontend demo on Vercel.

## How to Save Files for Real (Next Step)
To actually store uploaded files, you would need a backend. The easiest free options are:

1. **Cloudinary** (free tier) — great for video/image hosting
   - Sign up at https://cloudinary.com
   - Use their Upload API in your JS

2. **Supabase Storage** (free tier) — open source, easy setup
   - Sign up at https://supabase.com
   - Add a Storage bucket and upload via their JS SDK

3. **Vercel Blob** — works natively with Vercel
   - Docs: https://vercel.com/docs/storage/vercel-blob

For now, uploaded files are stored in memory while the page is open.
