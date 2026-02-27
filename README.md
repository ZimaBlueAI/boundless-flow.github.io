# boundless-flow.github.io

Official documentation & landing site for **Boundless Flow (无界音流)**.

🌐 **Live site:** https://boundless-flow.github.io/

## Repo structure

```
.
├── index.html                    # Landing page (中文)
├── index-en.html                 # Landing page (English)
├── welcome.html                  # Docs – What is Boundless Flow? (中文)
├── welcome-en.html               # Docs – What is Boundless Flow? (EN)
├── stt.html / stt-en.html        # Real-time STT
├── translation.html / -en.html   # Real-time Translation
├── proofreading-summary.*html    # AI Proofreading & Summary
├── tts-voice-cloning.*html       # TTS & Voice Cloning
├── appendix.html / -en.html      # Appendix / Beginner guide
├── style.css                     # Shared stylesheet
├── images/                       # Screenshots & illustrations
│   ├── banner.png
│   ├── img1.png … img9.png
└── .nojekyll                     # Disable Jekyll processing
```

## Deploy to GitHub Pages

1. **Create the repo** as `boundless-flow/boundless-flow.github.io`  
   (the special `<username>.github.io` naming makes GitHub Pages serve the site directly at `https://boundless-flow.github.io/`).

2. Push this folder as the `main` branch root:
   ```bash
   git init
   git remote add origin https://github.com/boundless-flow/boundless-flow.github.io.git
   git add .
   git commit -m "chore: initial site publish"
   git push -u origin main
   ```

3. In the repo **Settings → Pages**:
   - Source: **Deploy from branch**
   - Branch: `main` / `(root)`
   - Save.

The site is live in ~1 minute.

## Syncing with the plugin source

Source docs live in  
`ai-whiteboard-next/plugins/boundless-flow/docs/`  

After editing docs there, re-sync with:
```powershell
Copy-Item -Path "plugins\boundless-flow\docs\*" `
          -Destination "..\..\boundless-flow.github.io\" `
          -Recurse -Force
```

## License

See [boundless-flow](https://github.com/ZimaBlueAI/boundless-flow) for the main project license.
