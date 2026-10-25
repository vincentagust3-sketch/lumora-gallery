LUMORA SOCIAL STARTER
Includes demo gallery, sign-up/sign-in UI, publish pin, download link, comments UI, save pins, profile section, dark/soft theme. Real online actions require Supabase configuration.

SETUP (later, when ready):
1. Create project at https://supabase.com/
2. Run setup.sql in SQL Editor.
3. Create a PUBLIC Storage bucket named lumora.
4. In index.html replace PASTE_SUPABASE_PROJECT_URL_HERE and PASTE_SUPABASE_ANON_KEY_HERE with your project URL and anon/public key. NEVER use a service-role key in browser code.
5. Host index.html on a static host to get a public URL.

Note: This is a starter, not a finished production social network. Before public launch, add upload moderation, rate limits, reporting, and profile creation trigger/verification. Supabase free-tier limits may apply. Only upload images you own or have permission to share. Demo mode does not create real accounts or save comments.

REELS SECTION:
The Reels tab includes demo videos and lets you preview a local video in your browser. Local reel previews are not uploaded or shared online and disappear when the page is refreshed. For public reels, add a Supabase videos table, storage bucket/policies, moderation, and upload playback support before launch.

ONLINE REELS SETUP (included in latest setup.sql and index.html):
- Run the full setup.sql in Supabase SQL Editor (if you ran an older version, run the new file too; if policies already exist, Supabase may report duplicate policy names).
- In Supabase Storage create a PUBLIC bucket named lumora-reels. Keep the browser code configured with the anon/public key only.
- Sign in to Lumora, open Reels, choose a video under 50 MB, and publish. Uploaded reels become visible to other visitors.
- Before a public launch, add moderation/reporting and review storage limits. This starter does not yet include reel likes, captions beyond a title, or content moderation.
