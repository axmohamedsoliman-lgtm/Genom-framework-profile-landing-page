# Landing Page — Add Your Screenshots Here

The landing page (`index.html`) is ready and will display screenshots automatically when images are placed in the correct folders.

## Where to Put Screenshots

```
landing-page/
└── images/
    ├── naomi-ai/           ← Add screenshot.png here (Naomi AI app)
    ├── clinic/             ← Add screenshot.png here (Genom Clinic)
    ├── modern-server/      ← Add screenshot.png here (Modern Server)
    ├── games/              ← Add screenshot.png here (I Identify as a Horse)
    ├── noir-audio-studio/  ← Add screenshot.png here (Noir Audio Studio)
    ├── noir-gif-studio/    ← Add screenshot.png here (Noir GIF Studio)
    ├── x-local/            ← Add screenshot.png here (X-Local)
    ├── mouse-overlay/      ← Add screenshot.png here (Mouse Overlay)
    └── genom-browser/      ← Add screenshot.png here (Genom Browser UI)
```

## How the Cards Work

Each app card in the landing page uses this pattern:
```html
<img src="images/{app}/screenshot.png"
     alt="App name"
     onerror="this.parentElement.innerHTML = '<placeholder>'">
```

If the image doesn't exist, a clean placeholder is shown automatically.

## Recommended Screenshots

- **Naomi AI**: The chat UI with a response being streamed
- **Genom Clinic**: The main dashboard or patient list
- **Modern Server**: The server management dashboard with live metrics
- **Games**: A gameplay moment from I Identify as a Horse
- **Noir Audio Studio**: The waveform editor
- **X-Local / GIF Studio**: The media gallery view

Any resolution works. The cards display them at 16:9 aspect ratio with `object-fit: cover`.
