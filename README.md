# Chat Video Editor V1

A free, static, browser-based video editing prototype. It runs FFmpeg.wasm in the browser and does not upload the selected video to a server.

## Run it
This project must be served from HTTPS or localhost (not opened as a `file://` URL).
The easiest free deployment is GitHub Pages:
1. Create a free GitHub account (if needed).
2. Create a public repository named `chat-video-editor`.
3. Upload `index.html` from this folder.
4. Open repository Settings → Pages.
5. Under Build and deployment, choose Deploy from a branch; select `main` and `/ (root)`, then Save.
6. Open the published HTTPS Pages address on your phone.

## Supported V1 commands
- `video ko 5 second se 20 second tak trim karo`
- `video mute karo`
- `video ko 720p mein resize karo`
You can combine these using the controls before exporting.

## Important
- First load needs internet to download FFmpeg.wasm from the CDN.
- Rendering uses phone RAM/CPU. Start with short, small MP4 files (e.g. 10–30 seconds).
- This is a prototype, not an AI scene-understanding editor. It does not yet do automatic highlight selection, object removal, generated effects, or advanced transitions.
- The command parser is local and rule-based; no paid AI API is used.
