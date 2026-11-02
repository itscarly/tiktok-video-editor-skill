# Local editing tools

On this Mac the editor's isolated Python is `~/.local/share/tiktok-video-editor/python/bin/python`, with faster-whisper and OpenCV contrib. The cached `small` Whisper model can be loaded by faster-whisper on CPU with int8; `word_timestamps=True` yields approximate word times. Review the transcript and boundaries against the audio before cutting. Model selection may be adjusted for accuracy and resources.

OpenCV's `TrackerCSRT_create` tracks an initialized bounding box, not a speaker's identity or speech. Select the subject based on reviewed footage, inspect loss and drift, correct the track, and smooth reframing; preserve useful context and review the vertical crop throughout.

Puppeteer is installed in `~/.local/share/tiktok-video-editor/node_modules`; scripts can resolve it from that directory and use installed Chrome via `executablePath`. Use it for browser-based graphics or frame capture where appropriate, then FFmpeg for encoding and assembly. HyperFrames may already handle browser capture; avoid duplicating it unnecessarily.

The environment uses PyAV 16.1.0 with faster-whisper 1.2.1; newer PyAV 19 failed audio decoding in testing. Verify dependencies on the current machine and explain failures. For setup use isolated environments; do not modify another skill's private environment.

The installed FFmpeg build lacks `drawtext` and `subtitles` filters. Check `ffmpeg -filters` before relying on them; render transparent text or caption layers through Puppeteer, HyperFrames, or another available editor and composite with FFmpeg. Review legibility and avoid duplicating captions already burned into source footage.
