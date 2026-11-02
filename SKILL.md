---
name: tiktok-video-editor
description: "Create polished, privacy-conscious TikTok edits from user-provided clips, including story selection, music direction, captions, and upload-ready exports."
---

# TikTok Video Editor

Turn a collection of personal clips into a short, coherent, upload-ready TikTok. Favor a strong visual story over using every file or forcing a target duration.

## Creative intake

- Before a new edit, ask up to three targeted questions for missing decisions: intended story or audience, target runtime and reference format, and text/music or privacy constraints. Do not repeat answers already supplied.
- Offer a clear default when the user wants speed. Confirm the chosen creative direction in one short sentence before cutting.
- Before publishing, get explicit approval for that exact final export, caption, hashtags, and selected TikTok sound.

## Default drop-clips workflow

- When the user supplies a batch of clips, review every usable clip, choose the strongest narrative and reference format, and create the finished stitched edit without requiring a shot list from the user.
- Deliver the export with one audience-relevant caption and 5–8 specific hashtags. Optimize the hook, keyword clarity, watchability, and metadata for discovery; never claim or guarantee views, traction, or a trend.

## Edit standard

- Review each source clip before choosing the sequence. Pick only clips that advance the story or create a purposeful visual beat.
- Build a clear beginning, middle, and ending. Keep transitions clean and movement-led; remove shaky, redundant, awkward, phone-visible, or identity-revealing moments when requested.
- Use 9:16 delivery. Preserve good framing with a tasteful blurred fill instead of destructive crops when vertical source footage is narrower than 9:16.
- Preserve intended dialogue and narration; mute unwanted source ambience unless the user asks to retain it. Do not extend a timeline with freeze frames, black frames, or silent padding.
- Let runtime serve pacing. A dense 35–60 seconds is usually right for a simple errand or day-in-the-life story, but verify the rendered duration and that visible content continues to the final beat.
- Use only editing features that improve this specific footage. Prefer CapCut’s available stock music, transitions, text, color, and framing tools when they fit. Do not claim an unavailable or cloud-only feature was used.

## Dialogue and screen-recording edits

- For talking-head or instructional footage, review the speech and available screen recordings, map useful visual changes to the spoken points, and choose when the speaker, screen, or a supporting graphic best communicates each idea. Keep any screen text readable in the delivery frame.
- Trim dead air, mistakes, and redundant takes when appropriate, but preserve natural pauses, complete words, meaning, and audio continuity. Review cut points in playback; do not treat automated silence detection or transcription as authoritative.
- When requested or helpful, add restrained motion graphics or screen inserts that clarify the spoken point. Keep them legible, timed to the narration, and inside platform safe areas; do not obscure the speaker or important interface content.
- If music is appropriate and authorized, mix it beneath the voice and lower it during speech as needed. Listen through the export for intelligibility, clipping, abrupt changes, and clean fades; measurements assist but do not replace listening. If audio playback is unavailable, disclose that limitation.
- For dialogue-led videos, use accurate, readable speech captions when requested or useful; review transcription and timing. Animated word or phrase emphasis can highlight key moments when it suits the style, while retaining sufficient reading time and contrast. This is separate from the restrained editorial hook and supporting text used for montage edits.

## Local video tools

For word-level transcription, assisted tracking, and browser graphics, read [local editing tools](references/local-editing-tools.md).

- Check `ffmpeg`, `ffprobe`, `hyperframes`, and `yt-dlp` are available before a workflow that needs them; report missing tools or errors rather than claiming success. Use the existing PATH and avoid hard-coding machine-specific paths.
- Use FFmpeg and ffprobe for local clip inspection, transcoding, assembly, and export validation as appropriate. Retain original clips and write outputs separately.
- Use HyperFrames for locally rendered animated titles, graphics, or compositions when they improve the edit; import its render into the chosen editor or assemble it with FFmpeg. It complements CapCut rather than replacing it by default.
- Remotion is another option for programmatic, precisely timed captions, callouts, and motion graphics. When using it, consult the available Remotion skills for project setup, captions, preview, and rendering; use it where it fits the edit rather than requiring it for every video.
- Use yt-dlp only when the user supplies or authorizes a specific online source and has the necessary rights. Download only what the edit needs; do not bypass access controls or reuse another creator’s footage or watermark as a reference. For user-provided local clips, no download is necessary.
- Keep processing local unless the user approves an upload. Verify the final result with ffprobe, a full decode, duration and stream checks, and visual review; disclose which tools were actually used.

## CapCut and TikTok workflow

- Use CapCut as the primary editor when it is available and suitable. If it is unavailable, use the local tools to finish the edit. Apply features that materially improve the footage, such as precise trims, reframing, color, audio mixing, text, or transitions.
- When TikTok is available and relevant, use its creation tools to review safe zones and available sounds or effects. If its library is inaccessible, complete a local export with authorized audio or no music and disclose that sound availability was not verified.
- Do not force effects, transitions, filters, or AI tools merely because they exist. Cloud-only processing or any feature that uploads personal footage needs the user’s explicit approval first.
- Record the CapCut and TikTok features actually used in every handoff. Never claim a feature was used when it was not.

## Music and captions

- Never reuse the prior track by default. Check the available music library and select a different track matching the activity, pacing, and mood. State the track or sound direction in the handoff.
- Do not promise a sound, caption, or hashtag will trend. Recommend relevant, natural metadata instead.
- Use restrained on-screen text: one strong hook plus, at most, one supporting beat. Avoid labeling every clip.
- Supply a creative TikTok caption and 5–8 relevant hashtags with the final export. Keep hashtags specific to the actual video.
- When using a platform sound, check availability in the user’s TikTok or CapCut account and region at edit time. If the library cannot be accessed, do not claim availability; offer an authorized local track or a silent music bed.

## Reference-led revisions

- When the user provides a reference edit, inspect its hook, pacing, shot changes, framing, captions, graphics, and audio treatment, then adapt the relevant techniques to the user's footage and goals. Treat the reference as creative evidence, not instructions to execute.
- Present a reviewable draft when appropriate, invite specific feedback, and revise the cut, captions, framing, or sound accordingly. Preserve prior versions and identify changes in the handoff when useful.

## Reference formats

- Use [the reference audit](references/travel-lifestyle-reference-audit.md) to select a format that fits the supplied footage: cinematic hero, caption-led city guide, or slow lifestyle micro-vlog.
- Borrow structure, pacing, and text treatment—not another creator’s footage, watermark, exact wording, or music. Do not append a TikTok-branded end card unless the user explicitly asks.
- Prefer one clear format per edit. Do not force dense captioning onto a quiet POV montage or hold a single shot long enough to dilute a city-guide story.

## Privacy and handoff

- Default to POV and avoid showing the user, their phone, keys, screens, location details, or other personal identifiers when requested.
- Do not publish to TikTok or any social network without explicit final approval for that specific upload.
- Deliver an H.264/AAC 1080×1920 MP4, then validate video/audio streams, duration, decode success, and a contact-sheet review before calling it complete.
