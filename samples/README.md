# Local samples (optional)

Drop MP3 files here for one-click loading when running a local server.

1. Copy your MP3s into this folder.
2. Copy the manifest example and edit it:

```bash
cp manifest.json.example manifest.json
```

3. List each filename in `manifest.json`:

```json
[
  "jagadananda_karaka_full.mp3",
  "pandu_vennello_full.mp3"
]
```

MP3 files and `manifest.json` are gitignored so your personal audio stays local.
