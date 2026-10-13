# Eduard Nesterov

**Junior ML Engineer** · Kyiv, Ukraine

Applied mathematics graduate building ML systems around local models: embeddings, clustering, classification and LLM text generation, all running on my own hardware, with no cloud APIs.

### Projects

**Telegram news autoposting system** · *private, built at Slavnyi Media Group*

A pipeline of 18 services that finds stories covered by several sources, rewrites them in a channel's style with a local LLM and publishes them on schedule.
- bge-m3 embeddings in pgvector, incremental clustering of posts into stories
- scikit-learn classifiers on embeddings: topic accuracy 74.9% vs 71.1% for the rule-based baseline (5-fold CV); a "not news" filter with zero false positives on a held-out human-labeled set
- similarity thresholds calibrated with precision–recall on blind-labeled pairs
- local LLM rewriting (Gemma 3 12B) with similarity-retrieved few-shot examples and an automatic validator that feeds errors back for a retry

**[vidloc](https://github.com/EduardNesterov/vidloc)** · *Python, MLX*

Translates video EN/RU/IT → Ukrainian on a Mac: Whisper for speech recognition, NLLB-200 / Aya for translation, StyleTTS2 / F5-TTS for dubbing, LaMa + CRAFT to remove watermarks and burned-in subtitles.

**[TrackpadPhone](https://github.com/EduardNesterov/TrackpadPhone)** · *Swift*

An iPhone as a trackpad and keyboard for a Mac: gesture recognition, inertia and an encrypted UDP channel, with no account and no cloud.

### Stack

- **ML / NLP:** embeddings, semantic search, clustering, classification, ranking, scikit-learn, NumPy
- **LLMs:** llama.cpp, MLX, GGUF quantization, prompt engineering, few-shot / RAG
- **Speech / CV:** Whisper, NLLB-200, StyleTTS2, F5-TTS, LaMa, CRAFT
- **Backend:** Python, FastAPI, asyncio, PostgreSQL + pgvector, Docker Compose, Prometheus, Linux

### Languages

Ukrainian, Russian (native) · English (B1)
