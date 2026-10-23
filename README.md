# Command Center

Private task dashboard (static page on GitHub Pages; data + login in Supabase, schema `command`, row-level security: owner only).

- Each task is its own chat thread: text, photos (resized to 1600px JPEG in the browser), PDFs, voice messages, reactions, pins, read receipts.
- Attachments live in a PRIVATE Supabase Storage bucket `command-attachments` (owner-only policies), shown through short-lived signed URLs.
- Desktop (1100px and wider): projects | tasks | chat. Phone and iPad: stacked pages.
- No secrets in this repo (the Supabase publishable key is public by design; access is enforced by RLS).
