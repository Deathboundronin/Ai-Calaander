# Calendar Butler

AI calendar with a voice butler. Installable app (PWA), optional cross-device sync.

## 1. Host it (GitHub Pages)
Create a repo (e.g. `calendar-butler`), upload everything in this folder, then Settings > Pages > Deploy from branch `main` / root.
Your app: `https://YOUR-USERNAME.github.io/calendar-butler/`

## 2. Give the butler a brain (cheap/free AI key)
Default is Google Gemini's free tier:
1. Go to aistudio.google.com > Get API key > Create key.
2. Put it in `config.js` as `AI_KEY`. If the model name is rejected, copy a current Flash / Flash-Lite model name from AI Studio into `AI_MODEL`.

Any OpenAI-compatible provider works. Change `AI_BASE_URL`, `AI_MODEL` and `AI_KEY`
(e.g. DeepSeek: `https://api.deepseek.com`, model `deepseek-chat`).

NOTE: the key sits in a public file, so anyone who opens your site's source can see it.
Fine for personal use on the free tier. Don't use a key with a card attached, and don't share the link widely.

## 3. Sync (optional)
Run `schema.sql` in your Supabase SQL Editor. `config.js` already has your Supabase URL and anon key.
Create an account in the sync card and sign in with the same email/password on each device.
If you host this next to Grit 75 on the same GitHub Pages account, you're already signed in.

## 4. Install
Edge/Chrome: install icon in the address bar. Phone: browser menu > Add to Home Screen / Install app.
