# Ringtone Trimmer

Browser-based MP3 ringtone trimmer with Apple-style drag handles. Load a track, set start and end on the waveform, preview the clip, and download a trimmed MP3. Everything runs locally in your browser; nothing is uploaded.

## Quick start

```bash
cd ~/Projects/code/ringtone-trimmer
python3 -m http.server 8765
```

Open [http://localhost:8765/](http://localhost:8765/)

You can also open `index.html` directly and use the file picker or drag-and-drop.

## Optional: local sample shortcuts

Put MP3s in `samples/` and list them in `samples/manifest.json` (see `samples/manifest.json.example`). When served over HTTP, those files show up as one-click chips on the load screen.

## How to trim

1. Load an MP3 (file picker, drag-and-drop, or sample chip).
2. Drag the **white side bars** to set start and end.
3. Drag the **yellow band** to slide the whole selection.
4. Use **Play selection** to preview.
5. Click **Download trimmed MP3**.

Fine-tune with the − / + steppers (0.1s) or type exact times.

## Stack

- [WaveSurfer.js](https://wavesurfer.xyz/) for waveform display
- Web Audio API + [lamejs](https://github.com/zhuker/lamejs) for MP3 export
- Single static HTML file, no build step

## License

MIT
