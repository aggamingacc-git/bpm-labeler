A fast, hybrid BPM detection and tagging tool for Windows.
BPM‑LABELER scans your music library, detects tempo using both online lookup and local audio analysis, writes BPM tags into your files, and generates a Missing API Matches report for tracks the API couldn’t identify.
This project is designed for accuracy, speed, and clean metadata — ideal for DJs, archivists, and anyone maintaining a large music library.

🚀 Features
Hybrid BPM Detection
- Online lookup via the GetSongBPM API
- Local BPM analysis using:
- Spectral flux onset detection
- Multi‑hop tempo estimation
- Downbeat analysis
- Autocorrelation confidence scoring
- Automatic double/half‑tempo correction
Metadata Integration
- Reads artist, title, and album tags
- Writes BPM tags back into:
- MP3 (ID3 TBPM)
- M4A/MP4 (tmpo)
- FLAC / OGG / Vorbis (BPM)
- WAV / AIFF (where supported)
Caching
- Avoids reprocessing files
- Stores BPM, confidence, and source (api/local/cache)
Batch Processing
- Recursively scans folders
- Processes thousands of files efficiently
- Generates:
- bpm_results.csv
- missing_bpm_api.csv
Polished UI
- Tkinter interface
- Progress/status updates
- Results table with:
- File
- Artist
- Title
- Album
- BPM
- Confidence
- Source
- Button to view Missing API Matches
- Background worker thread (non‑blocking UI)
