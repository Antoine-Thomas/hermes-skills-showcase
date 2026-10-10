# Hermes Skills Showcase

**Security-reviewed · Available on Agensi.io**

A curated pack of [Hermes Agent](https://hermes-agent.nousresearch.com/) skills for **AI video
automation**, **free-model routing** and **Windows system optimisation**. The pack turns a local
Windows workstation into a reproducible AI-video pipeline: voice cloning, face animation, final
assembly, and cost-aware LLM routing — each step a documented, self-contained skill.

This repository is a **showcase only** — it demonstrates the workflow, commands and outputs.
The full, working source (Python + PowerShell + FFmpeg pipelines) ships with the commercial version.

---

## What's included in the full version

- **ai-video-pipeline** — end-to-end AI video inference & assembly, with the 8 GB VRAM rules
  (RTX 3070 Ti) and the 4K H.265 delivery spec
- **liveportrait-pipeline** — realistic face animation (LivePortrait), GPU tuning, background/logo composite
- **talking-head-video** — full SadTalker + LivePortrait + assembly pipeline
- **video-youtube-assembly** — final assembly: animated background + logo + audio + title
- **tts-voice-cloning** — French voice cloning with XTTS-v2
- **omniroute-auto-update** — auto-discovery of new free AI models with Telegram notification
- **nvidia-nim-vision** — vision via NVIDIA NIM (local proxy + API)
- **windows-optimization** — temp cleanup, scheduled-task management, Windows tuning
- **security-monitoring** — detect monitors that spam or miss alerts

## Live preview

**Voice + talking head**

```bash
$ hermes run talking-head-video --photo portrait.jpg --audio voice.wav
✓ XTTS-v2 voice rendered (fr, temp 0.75)
✓ SadTalker 512px driving video
✓ LivePortrait refinement (--source-max-dim 512)
✓ Face animation rendered at 11.1x realtime
✓ Output: talking_head.mp4
```

**Final assembly**

```bash
$ hermes run video-youtube-assembly --music track.mp3 --logo logo.png --title "Episode 3"
✓ Background looped to audio length
✓ Logo + title overlay applied
✓ H.265 CRF 18 mux  →  final.mp4 (3840×2160, ~45 Mbps)
```

**Free-model routing**

```bash
$ hermes run omniroute-auto-update
✓ Checked provider catalogue
✓ 3 new free models added to the `eco` combo
✓ Telegram notification sent
```

See [`examples/`](examples/) for the full before/after write-ups.

## Requirements

- Hermes Agent v0.21+ (https://github.com/NousResearch/hermes-agent)
- Python 3.11+
- FFmpeg on `PATH` (video skills)
- GPU recommended (RTX 3070 Ti / 8 GB VRAM profile included for video/IA tasks)
- Optional API keys: OmniRoute, NVIDIA NIM, OpenAI (see each skill's `.env.example`)

## Buy the full version on Agensi

**https://www.agensi.io/@thomas-leroyer**

## About the author

Thomas Leroyer — searching.murphy@gmail.com

## License

Copyright (c) 2026 Thomas Leroyer. All rights reserved.

This repository is a showcase only. The code, scripts, and skill files presented here are
proprietary and may not be copied, modified, distributed, sublicensed, or used commercially
without explicit written permission from the author. See [`LICENSE`](LICENSE).

To purchase a commercial license: https://www.agensi.io/@thomas-leroyer

---

**Keywords**: Hermes Agent skills, video automation, FFmpeg, talking-head video, voice cloning,
system optimization, Windows automation, AI agent workflow.
