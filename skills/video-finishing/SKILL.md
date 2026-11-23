---
name: video-finishing
description: Edit AI Editor video takes or assembled Shorts, synchronize captions and sound, and verify a review or release export.
---

# Video finishing

1. Inspect the take and its audio with FFprobe. Transcribe locally when the edit needs a dialogue map. In AI Editor, use `transcribe.py` with the project Python environment. Preserve intentional pauses and trim dead air and retakes before locking captions.
2. Build captions from the edited dialogue and correct names and terminology against the audio. For doomv12, use short bold white phrases with a dark outline and selective green or gold emphasis. Place them in the lower third clear of faces and the Shorts controls. Keep the voice intelligible over music and effects.
3. Use the existing renderer for a project composition. Use FFmpeg for simple cuts, assembly, or subtitle burns. Run the project's validation command when it has one.
4. Export a versioned H.264/AAC MP4 and synced SRT when dialogue is captioned. Verify dimensions, duration, decoding, and audio levels. Inspect frames at the opening, each important transition, and the ending, and check caption timing on playback. AI Editor exports go to `done/<channel>/`.
