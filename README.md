# MPI Ekonomi — Permintaan
## Struktur Project

```
mpi-permintaan/
├── index.html           ← File utama (SATU file, selalu edit di sini)
├── generate_audio.py    ← Generate ulang semua file audio
├── assets/
│   └── audio/
│       ├── intro-bg.wav
│       ├── sesi1-bg.wav
│       ├── btn-click.wav
│       ├── timer-start.wav
│       ├── tick.wav
│       ├── tick-urgent.wav
│       ├── timer-end.wav
│       ├── correct.wav
│       └── wrong.wav
└── README.md
```

## Setup VSCode (sekali saja)

1. Install extension **Live Server** (Ritwick Dey)
2. Klik kanan `index.html` → **Open with Live Server**
3. Browser terbuka di `http://127.0.0.1:5500`
4. Setiap `Ctrl+S` → browser auto-refresh otomatis

## Generate Audio (jika file audio hilang)

```bash
pip install numpy
python generate_audio.py
```

## Workflow Update Code

1. Edit `index.html` di VSCode
2. `Ctrl+S` → Live Server auto-refresh
3. Tidak perlu download ulang file HTML

## Cara Menambah Sesi Baru

Tambahkan section di `index.html` dengan pola yang sama:
- HTML: `<div id="s2">...</div>` di dalam `#ga`
- CSS: style untuk `#s2`
- JS: fungsi `startS2()`, `loadCaseS2()` dll
