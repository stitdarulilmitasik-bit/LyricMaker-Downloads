# LyricMaker

**LyricMaker** is an Android lyric-video editor for combining music, synchronized lyrics, photos or videos, typography, and audio-reactive visualizers into MP4 videos.

The editor is being developed around a mobile video-editing workflow: a large preview, persistent playback controls, and clearly separated tools that are easy to reach.

## Current development progress

### Editor interface — latest update

The editor navigation and tool layout have been reorganized to make common actions easier to access:

- **Media** — opens the device media picker to choose a photo or video background.
- **Audio** — opens the audio picker directly.
- **Lirik (Lyrics)** — opens the lyrics import flow. TXT, SRC, and LRC files are supported.
- **Style** — opens lyric typography and appearance controls.
- **Timeline** — opens lyric timing controls and line-by-line synchronization tools.
- A persistent mini audio player remains available at the bottom of the editor, with playback, seek, and restart controls.
- The preview window no longer contains the old Photo/Video or Add Media buttons. Media selection is handled through the **Media** navigation tool.
- The old **Audio & Sync** browser panel has been removed. Audio selection is now a direct tool, while synchronization is accessed from the Timeline workflow.
- The lyrics panel is presented as **Lirik**, with a dedicated **Insert Lirik** action.

### Synchronization workflow

- Open **Timeline** to view lyric lines and their current timestamps.
- Select a line and use its **SYNC** action to set its timing at the current audio position.
- Use **Sync** in the Timeline header to open the synchronization workspace.
- The synchronization workspace provides playback, manual SYNC, start/finish sync, and AI Sync controls.
- Reset Timing remains available from Timeline.

## App capabilities

- Audio selection and playback preview.
- Lyrics import and editing (TXT, SRC, and LRC).
- Manual line-by-line lyric synchronization.
- AI Sync workflow.
- Timeline view with line selection and timestamp editing.
- Primary and secondary lyric line styling, including separate colors.
- Font family, font style, font size, and color controls.
- Photo/video backgrounds.
- Audio-reactive visualizer for preview and export.
- MP4 video export with export progress.
- Save and open project workflows.
- Persistent playback controls and editor tool navigation.

## Latest source update and build status

The latest editor changes have been committed to the private source repository.

- Latest UI commit: `8968ee3` — Keep lyric synchronization accessible from timeline tools.
- Previous UI commits:
  - `3bc413e` — Remove photo and video actions from preview placeholder.
  - `7ec7656` — Replace editor browsers with direct media audio and lyrics tools.
  - `5b3ad64` — Correct editor tool navigation scroll targets.
- GitHub Actions build **#220** was still running when the source README was updated. A successful build and release had not yet been confirmed at that time.

[View the source repository's latest GitHub Actions run](https://github.com/stitdarulilmitasik-bit/Video_Lyrics_Maker_Android/actions/runs/38909230969)

## Download

Get the latest Android release from the public Releases page:

**[Download LyricMaker](https://github.com/stitdarulilmitasik-bit/LyricMaker-Downloads/releases)**

Release files may include:

- **APK** — install directly on a compatible Android device.
- **AAB** — Android App Bundle intended for distribution through Google Play.

For the latest available version, use the newest release listed on the Releases page.

## Compatibility

- Minimum Android SDK: 26.
- Current native release ABI: `arm64-v8a`.

## Release and source repositories

The application source code is maintained in a separate private repository:

[Video_Lyrics_Maker_Android](https://github.com/stitdarulilmitasik-bit/Video_Lyrics_Maker_Android)

This public repository is used for distributing Android release files and publishing user-facing release information. It does not contain the private application source code or release-signing credentials.

Android release builds are produced through GitHub Actions. Release signing credentials are stored as protected repository secrets and are not included in this public repository.

## Project status

LyricMaker is under active development. The editor interface has recently been reorganized, and timeline synchronization, visualizer export smoothness, and overall release validation remain ongoing improvement areas.

Features and export behavior may continue to improve between releases.
