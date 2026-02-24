# Wav2Pwn — Extra Evaluation Demo

Supplementary evaluation results and audio demos for **Wav2Pwn: A Framework for Targeted Black-Box Attacks on Self-Supervised Learning Based Speech Recognition Models** (AsiaCCS 2026).

## GitHub Pages setup

1. Push this repo to GitHub.
2. In the repo: **Settings → Pages**.
3. Under "Build and deployment", choose **Deploy from a branch**.
4. Branch: `main` (or your default), folder: **/ (root)**.
5. Save. The site will be at `https://<username>.github.io/<repo>/`.

## Adding your content

- **Audio files:** Put your `.wav` files in the `audio/` folder with these names:
  - `Original_audio_1.wav`, `Original_audio_2.wav`
  - `Adversarial_audio_1.wav` … `Adversarial_audio_8.wav`
- **Paper link:** In `index.html`, set the `href` of the "Paper (AsiaCCS 2026)" link to your PDF URL (e.g. upload the PDF to the repo or use a conference link).
- **Metrics:** Replace the "—" placeholders in the tables with your extra evaluation results (Generated Adversarial Text, TASR, UASR, Clean CER %, Avg UASR, Avg TASR, SNR dB) when ready.

## Local preview

Open `index.html` in a browser, or run a simple server:

```bash
python3 -m http.server 8000
```

Then visit `http://localhost:8000`. For audio to load, you must use a server (file:// may block loading audio).
