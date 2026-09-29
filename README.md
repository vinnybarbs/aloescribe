# Aloe Scribe

The private meeting notepad. Records, transcribes, labels speakers, and
summarizes meetings entirely on your machine. No bot, no cloud, no
account, and nothing ever leaves your computer.

Website and downloads: [aloescribe.ai](https://aloescribe.ai)

This repository hosts the website, the signed release downloads, and the
AI model files the app fetches during its one-time setup. The application
source is maintained privately. Verify the privacy claim the strongest way
there is: put your machine in airplane mode and record an in-person
meeting. Transcription, speaker labels, and the summary all still happen,
because everything runs on your computer. Your video call needs the
internet. Aloe Scribe never does.

Security policy and vulnerability reporting: [aloescribe.ai/security](https://aloescribe.ai/security.html)

## Models hosted here

The app's one-time setup downloads these from the `model-*` releases with
checksum verification. Nothing is fetched from Hugging Face at runtime.

| Release | What | Size | License |
|---|---|---|---|
| model-parakeet-tdt-0.6b-v3 | Speech recognition, Parakeet TDT 0.6B v3 (NVIDIA, MLX) | 2.4 GB | CC-BY-4.0 |
| model-gemma-4-26b-a4b-4bit | Meeting summaries, high quality, Gemma 4 26B-A4B (Google, 4-bit MLX), Macs with 32 GB or more | 14.3 GB | Apache 2.0 |
| model-qwen3.5-9b-mlx-4bit | Meeting summaries, standard, Qwen3.5 9B (4-bit MLX), 16 GB Macs | 6.0 GB | Apache 2.0 |
| model-qwen3.5-4b-mlx-4bit | Meeting summaries, compact, Qwen3.5 4B (4-bit MLX), 8 GB Macs | 3.1 GB | Apache 2.0 |
| model-qwen3.6-35b-a3b-4bit-dwq | Previous high quality tier, kept for installs that have it | 20.7 GB | Apache 2.0 |

Each release carries a SHA256SUMS manifest and, for the summary models, a
NOTICE.txt with the source and license.
