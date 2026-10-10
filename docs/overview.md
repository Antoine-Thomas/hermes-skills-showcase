# Overview

Hermes Skills is a pack of [Hermes Agent](https://hermes-agent.nousresearch.com/) skills that
turns a local Windows workstation into a reproducible **AI video factory** and a
**cost-aware LLM router**.

Two themes run through the pack:

1. **Local-first AI video** — clone a voice, animate a portrait, assemble a 4K deliverable with
   FFmpeg, all on a single consumer GPU (RTX 3070 Ti / 8 GB VRAM).
2. **Free-first model routing** — discover new free models automatically and keep the agent's
   fallback chain cheap before anything paid is hit.

## The skills

| Skill | Theme | What it does |
|-------|-------|--------------|
| `ai-video-pipeline` | Video | End-to-end inference + assembly, 8 GB VRAM rules, 4K H.265 spec |
| `liveportrait-pipeline` | Video | Face animation, GPU tuning, composite |
| `talking-head-video` | Video | SadTalker + LivePortrait + assembly |
| `video-youtube-assembly` | Video | Background + logo + title + audio mux |
| `tts-voice-cloning` | Audio | XTTS-v2 French voice cloning |
| `omniroute-auto-update` | Routing | Free-model discovery + Telegram alert |
| `nvidia-nim-vision` | Vision | NIM local proxy + API |
| `windows-optimization` | System | Temp cleanup, scheduled tasks, tuning |
| `security-monitoring` | System | Detect noisy / silent monitors |

## Why a "pipeline" and not one script

Each stage is its own skill so an agent can run, pause, inspect and resume a long render — the
video path is minutes-to-hours, and a single monolithic script makes partial failure expensive.
Splitting it also lets you swap one stage (e.g. a different TTS) without rewriting the rest.

> This repository is the **showcase**: it documents behaviour and shows real-looking commands and
> outputs. The executable source is the paid product.
