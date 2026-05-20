PANDUAN ASET SUARA - Slide Master Puzzle
=========================================

Letakkan file suara berikut di folder ini (resources/sounds/):

1. slide.wav atau slide.mp3
   → Suara saat menggeser tile puzzle
   → Rekomendasi: suara klik/woosh pendek (0.1-0.3 detik)

2. click.wav atau click.mp3
   → Suara saat mengklik tombol menu
   → Rekomendasi: suara tap pendek (0.05-0.1 detik)

3. win.wav atau win.mp3
   → Suara saat berhasil menyelesaikan puzzle
   → Rekomendasi: fanfare/jingle gembira (1-3 detik)

4. backsound.wav atau backsound.mp3
   → Musik latar belakang (looped otomatis)
   → Rekomendasi: musik instrumental ringan

Format yang didukung: WAV (paling kompatibel), MP3 (butuh SPI/JLayer)
Untuk MP3, tambahkan JLayer library ke classpath.

Jika file tidak ditemukan, game akan menggunakan suara sintetis (beep) sebagai fallback.
