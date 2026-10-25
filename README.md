# Storyforge RPG — custom website starter

This is a custom, mobile-first story/RPG interface you own and can publish as a static website. It includes character cards, scenario and world notes, saved chat history, edit/regenerate controls, import/export, and a story image gallery.

## Free AI connection
Text generation uses the AI Horde OpenAI-compatible API. Image generation uses the AI Horde image API. No paid API is configured, and the app itself has no subscription or paid-credit requirement. Anonymous access uses AI Horde's public anonymous key at the lowest priority; adding your own free AI Horde key can improve queue priority.

AI Horde is volunteer-powered, so generation speed and availability are not guaranteed. Free does not mean unlimited compute, and the upstream models/workers determine what content they will produce. Do not put private or sensitive personal information in prompts.

## Publish it free with GitHub Pages
1. Download and extract `storyforge-rpg-starter.zip`.
2. In a browser, open GitHub and create a new repository named `storyforge-rpg`. Set it to **Public** and create it.
3. In the new repository choose **Add file → Upload files**. Upload the four files in this folder: `index.html`, `style.css`, `app.js`, and `manifest.webmanifest` (you may also upload this README).
4. Open the repository's **Settings → Pages**.
5. Under **Build and deployment**, choose **Deploy from a branch**. Choose branch `main` and folder `/(root)`, then press **Save**.
6. Wait until GitHub Pages displays the published URL, normally `https://YOUR-USERNAME.github.io/storyforge-rpg/`. Open that URL in Chrome on your Android phone.
7. In the website, tap the gear icon, optionally enter a free AI Horde key, and tap **Refresh available text models**. If no key is entered, the site attempts anonymous access.

## Use it
- Create or edit character cards in **Characters**.
- Set the scene and the continuity notes in **Story RPG**, then tap **Start / continue story**.
- Enter your next action in the message box. Regenerate the last character reply or edit the last message when needed.
- In **Story Images**, write a prompt and generate an image. Generation may queue. Download completed images you want to keep.
- Use **Export all story data (JSON)** in Settings as a backup.

## Important current limitations
- Data is stored in the current browser/device, not a cloud database; separate devices do not automatically sync.
- Public static hosting means the source code and client-side app are visible. Do not store private API keys on a site you share publicly. For private personal use, keep your repository private (note: GitHub Pages availability for private repos depends on your GitHub plan) or use anonymous access.
- Persistent memory in this version means saved character cards, notes, and recent chat history are sent as context to the model; it is not an unlimited long-term memory system.
- Character image consistency is not automated. Reuse a portrait reference description in prompts to help consistency.
- This package is the website source, not yet a published live URL. No GitHub account or repository has been accessed or changed by this process.
