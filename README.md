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


## Tutorial: Cara Menambahkan dan Melakukan Sync Lirik

Ikuti langkah berikut untuk memasukkan lirik lagu, menyelaraskan setiap baris dengan audio, lalu membuat video lirik.

### 1. Masukkan audio lagu

1. Buka **LyricMaker** dan masuk ke halaman editor.
2. Pilih menu **Audio**.
3. Pilih file lagu dari penyimpanan perangkat.
4. Gunakan tombol Play pada pemutar audio untuk memastikan lagu sudah terbaca dan dapat diputar.

### 2. Masukkan file lirik

1. Pilih menu **Lirik (Lyrics)**.
2. Tekan **Insert Lirik** untuk memilih file lirik.
3. Pilih file berformat **.TXT**, **.SRC**, atau **.LRC**.
4. Periksa teks lirik yang tampil. Pastikan urutan baris sesuai dengan lagu.

**Catatan format:**
- **TXT/SRC**: berisi teks lirik per baris. Waktu kemunculan tiap baris perlu dibuat melalui proses sync.
- **LRC**: dapat memuat timestamp. Timestamp yang sudah ada akan dibaca oleh aplikasi dan dapat diperiksa atau disesuaikan melalui Timeline.

### 3. Buka Timeline

1. Pilih menu **Timeline**.
2. Daftar baris lirik akan ditampilkan bersama informasi waktunya.
3. Baris yang sudah memiliki waktu ditandai **Tersinkron**, sedangkan baris yang belum memiliki waktu ditandai **Menunggu**.
4. Tekan **Sync** pada bagian header Timeline untuk membuka ruang kerja sinkronisasi.

### 4. Lakukan sync manual dengan tombol REC / SYNC

Cara ini digunakan untuk merekam waktu mulai dan selesai setiap baris lirik mengikuti lagu.

1. Di ruang kerja Sync, tekan **Mulai Sync**. Audio akan mulai diputar jika belum berjalan.
2. Dengarkan lagu dan perhatikan baris lirik yang sedang dinyanyikan.
3. Saat penyanyi mulai mengucapkan baris tersebut, **tekan dan tahan tombol REC / SYNC**.
4. Tahan selama baris lirik dinyanyikan.
5. Saat baris tersebut selesai, **lepaskan tombol REC / SYNC**.
6. Aplikasi menyimpan waktu mulai dan selesai baris tersebut, kemudian berpindah otomatis ke baris berikutnya.
7. Ulangi langkah yang sama sampai semua baris selesai disinkronkan.
8. Tekan **Selesai Sync** setelah proses selesai.

**Indikator REC:** LED merah menyala ketika tombol REC / SYNC sedang ditekan. Lepaskan tombol pada akhir baris agar aplikasi mencatat batas akhir dan menyiapkan baris berikutnya.

### 5. Kontrol yang tersedia di ruang Sync

- **Play/Pause**: memulai atau menjeda audio.
- **REC / SYNC**: tekan dan tahan untuk menandai awal hingga akhir baris lirik.
- **Sebelumnya/Berikutnya**: berpindah di antara baris yang sudah memiliki waktu.
- **Mulai Sync**: memulai sesi sync baru.
- **Selesai Sync**: mengakhiri mode sync tanpa menghapus waktu yang sudah direkam.
- **AI Sync**: menjalankan bantuan sinkronisasi otomatis. Periksa kembali hasilnya karena timing otomatis mungkin masih perlu dikoreksi.

### 6. Periksa dan koreksi timing di Timeline

1. Kembali ke **Timeline** setelah menekan **Selesai Sync**.
2. Putar lagu dan periksa apakah setiap baris muncul sesuai suara penyanyi.
3. Pilih baris yang waktunya belum tepat.
4. Gunakan tindakan **SYNC** pada baris tersebut untuk menetapkan timing pada posisi audio saat ini.
5. Periksa kembali timestamp dan status setiap baris.

### 7. Simpan project dan ekspor video

1. Simpan pekerjaan menggunakan fitur **Save Project** agar proyek dapat dibuka dan dilanjutkan kembali.
2. Buka preview untuk memeriksa sinkronisasi, tampilan lirik, warna, font, dan latar belakang.
3. Atur gaya tampilan lirik sesuai kebutuhan.
4. Jalankan **Export** untuk membuat video MP4.
5. Tonton hasil ekspor untuk memastikan timing lirik sesuai dengan audio.

### Tips agar sync lebih akurat

- Gunakan earphone/headphone agar awal dan akhir pengucapan lebih mudah didengar.
- Lakukan sync di tempat yang tenang.
- Ikuti suara vokal, bukan hanya ketukan musik.
- Jangan menekan REC terlalu cepat atau melepasnya terlalu lambat.
- Periksa ulang bagian jeda, intro, outro, dan baris yang dinyanyikan cepat.
- Simpan project sebelum melakukan perubahan besar.

> **Penting — perhatikan sebelum memulai ulang:** tombol **Mulai Sync** memulai sesi baru dan menghapus timing lirik yang sudah ada. Jika hanya ingin menghentikan sesi dan mempertahankan hasil sync, gunakan **Selesai Sync**. Fitur **Reset Timing/Reset** di Timeline juga menghapus timing yang tersimpan. Pastikan Anda memang ingin mengulang dari awal sebelum menggunakan Mulai Sync atau Reset.

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
