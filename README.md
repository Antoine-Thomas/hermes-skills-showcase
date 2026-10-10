# Hermes Skills Showcase

[Security-reviewed · Available on Agensi.io]

## Summary

A curated collection of Hermes Agent skills for video automation, system optimization, and WordPress automation. This showcase presents selected capabilities designed to demonstrate the power and flexibility of the Hermes Agent platform.

## What's included in full version

- Video automation skills (LivePortrait, SadTalker, FFmpeg assembly)
- System optimization and Windows task management
- WordPress installation, backup, and deployment skills
- AI integration skills (OmniRoute auto-update, NVIDIA NIM vision, XTTS voice cloning)
- OmniRoute automatic updates with free AI model selection
- Telegram notification integration

## Live preview

### Example 1: OmniRoute Auto-Update
```
$ hermes run omniroute-auto-update
✓ Checking for new free AI models...
✓ Found 3 new accessible models
✓ Updated configuration with Gemini 2.0 Flash
✓ Notification sent to Telegram
```

### Example 2: LivePortrait Face Animation
```
$ hermes run liveportrait-pipeline --source phototetepourHErmesANIMA.jpg --audio ZOOM0004.WAV
✓ Processing started
✓ Face animation rendered (11.1x realtime)
✓ Video assembled with background music
✓ Output: output_video.mp4 (31.2 GiB RAM peak)
```

### Example 3: WordPress Site Creation
```
$ hermes run local-flywheel-setup --site-name "demo-site" --php-version "8.2"
✓ Local by Flywheel environment detected
✓ WordPress 6.6 installed
✓ Admin user created
✓ Site accessible at http://localhost:8080
```

## Requirements

- Hermes Agent v0.21.5 or later
- Python 3.11+ (for skill execution)
- GPU recommended for video processing skills
- API keys for OmniRoute, NVIDIA, or OpenAI (optional for basic skills)
- Local by Flywheel for WordPress skills

## Buy full version on Agensi

[Purchase commercial license on Agensi.io](https://www.agensi.io/@thomas-leroyer)

## About author

Thomas Leroyer — searching.murphy@gmail.com

## License

Copyright (c) 2026 Thomas Leroyer. All rights reserved.

This repository is showcase only. Code, scripts, and skill files presented
Here are proprietary and may not be copied, modified, distributed, sublicensed,
Or used commercially without explicit written permission from author.

To purchase commercial license, visit: https://www.agensi.io/@thomas-leroyer
Contact: searching.murphy@gmail.com