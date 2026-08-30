# recite-archive

Insurance copies of everything the "Recite with me" engine builds from, in
case any upstream vanishes. See `docs/recite-library.md` in the
new-muslim-guide repo for the whole picture, and `SHA256SUMS` here to verify
any file.

- `tarteel-ai/` — full Hugging Face snapshots of whisper-base-ar-quran and
  whisper-tiny-ar-quran (Apache-2.0). The `pytorch_model.bin` weights are on
  the release, not in git (GitHub's 100 MB limit).
- `ggml/` — the GGML conversions the app downloads (release assets), plus the
  Silero VAD model.
- `tools/convert-h5-to-ggml.py` — whisper.cpp's converter: originals + this
  file = fresh GGML forever.

Licences: Tarteel models Apache-2.0 (attribution kept); Silero VAD MIT;
converter MIT (whisper.cpp).
