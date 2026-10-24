# GolfCart Media firmware updates

Firmware downloads for the GolfCart Media steering-wheel controller. This public repository contains application firmware and release manifests/checksums only. Source, device settings and signing keys are maintained separately.

## Pick the correct board

- `gcmc-lcd128.bin`: Waveshare ESP32-S3 Touch LCD1.28, 240×240.
- `gcmc-amoled143.bin`: Waveshare ESP32-S3 Touch AMOLED1.43, 466×466.

Never install one board’s image on the other. Firmware1.6.0 or newer can check this repository over internet Wi-Fi and install a newer version after approval under Settings → Management → Firmware Updates. Older firmware needs one USB/local-portal bootstrap first. Checks do not turn Wi-Fi on or install automatically.

[Latest firmware downloads](https://github.com/droptopgokart/GolfCart-Media-Updates/releases/latest) · [Update manifest](https://github.com/droptopgokart/GolfCart-Media-Updates/releases/latest/download/update-manifest.json)

Each normal release carries both images, `update-manifest.json` and `SHA256SUMS.txt`. Manifests pin exact versioned HTTPS URLs, board image versions, sizes and SHA-256 checksums. Published versioned image bytes must never be replaced.

Check each release’s notes for validation status. The first1.6.0 release has software/host validation; real hardware OTA testing awaits connected controllers.
