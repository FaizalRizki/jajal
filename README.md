# Slide Master Puzzle

Game puzzle slide interaktif berbasis Java Swing.

## Struktur Package

```
src/
├── gameplay/        # Main, Window, Game, GamePanel, PuzzlePanel
├── gamestate/       # MenuPanel (sidebar), WinDialog
├── level/           # LevelConfig (enum), LevelSelectDialog
├── imageupload/     # ImageManager, SavedImage, ImageGalleryDialog
├── timer/           # GameTimer, MoveCounter
├── score/           # ScoreRecord, ScoreManager, ScoreBoard
├── settings/        # SoundManager, SoundSettingsPanel
└── ui/              # RoundedButton, StyledDialog, NotificationManager
```

## Cara Menjalankan di NetBeans

1. **File > Open Project** → pilih folder `SlideMasterPuzzle`
2. NetBeans akan mendeteksi `nbproject/` otomatis
3. Klik **Run Project (F6)**

## Cara Menjalankan Manual (javac + java)

```bash
cd SlideMasterPuzzle
mkdir -p build data/images

# Compile semua file Java
find src -name "*.java" | xargs javac -d build -sourcepath src

# Jalankan
java -cp build gameplay.Main
```

## Alur Permainan

1. Klik nama pemain (kiri atas) → isi nama → OK
2. Klik **Unggah Gambar** → pilih gambar dari komputer → klik thumbnail untuk memilih
3. Klik **Mulai Permainan** → puzzle teracak otomatis
4. Gerakkan tile dengan klik → timer & langkah mulai berjalan
5. Saat selesai → dialog "Kerja Bagus" muncul
6. Lihat papan skor lewat tombol **Papan Skor**

## Fitur

- 4 tingkat: Easy (3×3), Normal (4×4), Hard (5×5), Extreme (8×8)
- Upload & simpan banyak gambar (galeri lokal)
- Papan skor dengan ranking & delete
- Notifikasi toast kanan atas
- Sound effect synthesized (beep) + kontrol volume
- Animasi slide tile
- Saving skor & gambar persisten (folder `data/`)
