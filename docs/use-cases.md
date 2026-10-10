# Use cases

## 1. Solo video creator — a talking-head episode without a camera

You have a portrait and a script. The pack clones the voice, animates the portrait, and assembles
the episode — no studio, no camera, all local.

```bash
hermes run tts-voice-cloning --script script.txt --reference voice_ref.wav
hermes run talking-head-video --photo portrait.jpg --audio episode.wav
hermes run video-youtube-assembly --music track.mp3 --logo logo.png --title "Episode 3"
```

## 2. Course / explainer production on one GPU

Batch a series of lessons overnight: the 8 GB VRAM profile keeps each stage inside memory, and the
pipeline is checkpointed so a crash doesn't lose the whole run.

```bash
hermes run ai-video-pipeline --batch lessons/ --profile 8gb-vram --out dist/
```

## 3. Keeping AI costs near zero

The router prefers free models. This skill watches provider catalogues, adds what's new to the free
combo, and pings Telegram — so the fallback chain stays free-first without manual upkeep.

```bash
hermes run omniroute-auto-update
```

## 4. Keeping a Windows build machine healthy

Weekly cleanup + scheduled-task hygiene + a monitor that complains when it goes quiet.

```bash
hermes run windows-optimization --clean-temp --optimize-tasks
hermes run security-monitoring --check-silence
```
