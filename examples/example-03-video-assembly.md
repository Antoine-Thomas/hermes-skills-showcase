# Example 03 — Final 4K assembly with FFmpeg

## Command

```bash
hermes run video-youtube-assembly --video talking_head.mp4 --music track.mp3 \
    --logo logo.png --title "Episode 3" --out final.mp4
```

## Output (truncated)

```text
✓ Background looped to audio length
✓ Logo + title overlay applied
✓ H.265 CRF 18 mux  →  final.mp4 (3840×2160, ~45 Mbps)
✓ ffprobe verify: 3840x2160 · 45 Mbps · 04:12
```

## Before / After

- **Before**: raw talking-head clip, no music, no branding, not delivery-ready.
- **After**: a branded 4K H.265 file meeting the delivery spec in one command.
- **Time saved**: manual NLE assembly (import, sync, overlay, export) → scripted, repeatable mux.

## Delivery spec targeted

- 3840×2160, H.265 CRF 18, 45–60 Mbps, AAC 320k
- Duration 180–300 s, file 800 MB – 2 GB
