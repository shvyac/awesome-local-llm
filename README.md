# Awesome Local LLM

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

[日本語版はこちら / Japanese](README.ja.md)

A curated list of useful **local LLM** resources — inference engines, desktop apps and chat UIs, local-first RAG / agents, fine-tuning, and tools for picking a model that fits your hardware. Prefer durable official / project URLs.

**Discovery list only** — not a benchmark or ranking. Check each model's license and your hardware (VRAM / RAM) before downloading. ⭐ badges show live GitHub star counts (via shields.io).

## Contents

- [Inference engines & runtimes](#inference-engines--runtimes)
- [Serving frameworks (GPU / server)](#serving-frameworks-gpu--server)
- [Apple Silicon, edge & special hardware](#apple-silicon-edge--special-hardware)
- [Desktop apps](#desktop-apps)
- [Chat UIs & front-ends](#chat-uis--front-ends)
- [Local-first RAG, knowledge & agents](#local-first-rag-knowledge--agents)
- [Fine-tuning](#fine-tuning)
- [Model selection & utilities](#model-selection--utilities)
- [Archived / inactive](#archived--inactive)
- [Related lists](#related-lists)
- [Contributing](#contributing)

---

## Inference engines & runtimes

Run models on your own PC (CPU and / or consumer GPU).

- [Ollama](https://ollama.com/) ![GitHub stars](https://img.shields.io/github/stars/ollama/ollama?style=flat&label=%E2%AD%90) - The most popular way to pull and run open models with one command; local REST API. ([GitHub](https://github.com/ollama/ollama))
- [llama.cpp](https://github.com/ggml-org/llama.cpp) ![GitHub stars](https://img.shields.io/github/stars/ggml-org/llama.cpp?style=flat&label=%E2%AD%90) - LLM inference in C/C++; home of the GGUF format and the engine behind many other tools.
- [LocalAI](https://localai.io/) ![GitHub stars](https://img.shields.io/github/stars/mudler/LocalAI?style=flat&label=%E2%AD%90) - OpenAI-compatible API server for LLMs, vision, voice, image, and video; no GPU required. ([GitHub](https://github.com/mudler/LocalAI))
- [llamafile](https://github.com/mozilla-ai/llamafile) ![GitHub stars](https://img.shields.io/github/stars/mozilla-ai/llamafile?style=flat&label=%E2%AD%90) - Distribute and run an LLM as a single cross-platform executable (Mozilla.ai).
- [Xinference](https://github.com/xorbitsai/inference) ![GitHub stars](https://img.shields.io/github/stars/xorbitsai/inference?style=flat&label=%E2%AD%90) - Unified, OpenAI-compatible inference API across llama.cpp, vLLM, SGLang, transformers, and more.
- [PowerInfer](https://github.com/Tiiny-AI/PowerInfer) ![GitHub stars](https://img.shields.io/github/stars/Tiiny-AI/PowerInfer?style=flat&label=%E2%AD%90) - High-speed LLM serving for local deployment on consumer GPUs.
- [ExLlamaV2](https://github.com/turboderp-org/exllamav2) ![GitHub stars](https://img.shields.io/github/stars/turboderp-org/exllamav2?style=flat&label=%E2%AD%90) - Fast inference library for running LLMs on modern consumer GPUs.

---

## Serving frameworks (GPU / server)

High-throughput engines for a workstation or on-prem server.

- [vLLM](https://docs.vllm.ai/) ![GitHub stars](https://img.shields.io/github/stars/vllm-project/vllm?style=flat&label=%E2%AD%90) - High-throughput, memory-efficient inference and serving engine. ([GitHub](https://github.com/vllm-project/vllm))
- [SGLang](https://github.com/sgl-project/sglang) ![GitHub stars](https://img.shields.io/github/stars/sgl-project/sglang?style=flat&label=%E2%AD%90) - High-performance serving framework for LLMs and multimodal models.
- [LMDeploy](https://github.com/InternLM/lmdeploy) ![GitHub stars](https://img.shields.io/github/stars/InternLM/lmdeploy?style=flat&label=%E2%AD%90) - Toolkit for compressing, deploying, and serving LLMs (TurboMind engine).

---

## Apple Silicon, edge & special hardware

- [MLX](https://github.com/ml-explore/mlx) ![GitHub stars](https://img.shields.io/github/stars/ml-explore/mlx?style=flat&label=%E2%AD%90) - Apple's array framework for Apple silicon. ([mlx-lm](https://github.com/ml-explore/mlx-lm) ![GitHub stars](https://img.shields.io/github/stars/ml-explore/mlx-lm?style=flat&label=%E2%AD%90) for running LLMs)
- [MLC LLM](https://llm.mlc.ai/) ![GitHub stars](https://img.shields.io/github/stars/mlc-ai/mlc-llm?style=flat&label=%E2%AD%90) - Universal deployment engine with ML compilation (phones, browsers, GPUs). ([GitHub](https://github.com/mlc-ai/mlc-llm))
- [exo](https://github.com/exo-explore/exo) ![GitHub stars](https://img.shields.io/github/stars/exo-explore/exo?style=flat&label=%E2%AD%90) - Run large models across a cluster of your own devices.
- [BitNet](https://github.com/microsoft/BitNet) ![GitHub stars](https://img.shields.io/github/stars/microsoft/BitNet?style=flat&label=%E2%AD%90) - Microsoft's official inference framework for 1-bit LLMs (CPU-friendly).
- [Lemonade](https://github.com/lemonade-sdk/lemonade) ![GitHub stars](https://img.shields.io/github/stars/lemonade-sdk/lemonade?style=flat&label=%E2%AD%90) - Local LLM server optimized for AMD GPUs and NPUs (Ryzen AI, Radeon; ROCm / Vulkan / ONNX).

---

## Desktop apps

All-in-one apps for downloading models and chatting offline.

- [LM Studio](https://lmstudio.ai/) - Popular desktop app for discovering and running local models (app is closed source; [lms CLI](https://github.com/lmstudio-ai/lms) ![GitHub stars](https://img.shields.io/github/stars/lmstudio-ai/lms?style=flat&label=%E2%AD%90) is open source).
- [Jan](https://jan.ai/) ![GitHub stars](https://img.shields.io/github/stars/janhq/jan?style=flat&label=%E2%AD%90) - Open-source ChatGPT alternative that runs 100% offline. ([GitHub](https://github.com/janhq/jan))
- [GPT4All](https://www.nomic.ai/gpt4all) ![GitHub stars](https://img.shields.io/github/stars/nomic-ai/gpt4all?style=flat&label=%E2%AD%90) - Run local LLMs on any device (Nomic). ([GitHub](https://github.com/nomic-ai/gpt4all))
- [textgen (formerly text-generation-webui)](https://github.com/oobabooga/textgen) ![GitHub stars](https://img.shields.io/github/stars/oobabooga/textgen?style=flat&label=%E2%AD%90) - Open-source desktop app for local LLMs with OpenAI / Anthropic-compatible API.
- [AnythingLLM](https://anythingllm.com/) ![GitHub stars](https://img.shields.io/github/stars/Mintplex-Labs/anything-llm?style=flat&label=%E2%AD%90) - Local-first desktop / self-hosted app with RAG and agents. ([GitHub](https://github.com/Mintplex-Labs/anything-llm))

---

## Chat UIs & front-ends

Connect to Ollama, llama.cpp, or any OpenAI-compatible endpoint.

- [Open WebUI](https://openwebui.com/) ![GitHub stars](https://img.shields.io/github/stars/open-webui/open-webui?style=flat&label=%E2%AD%90) - Feature-rich self-hosted web UI for Ollama and OpenAI-compatible APIs (RAG, MCP). ([GitHub](https://github.com/open-webui/open-webui))
- [LobeHub](https://github.com/lobehub/lobehub) ![GitHub stars](https://img.shields.io/github/stars/lobehub/lobehub?style=flat&label=%E2%AD%90) - Agent workspace / chat UI (formerly Lobe Chat) supporting local and cloud models.
- [Cherry Studio](https://github.com/CherryHQ/cherry-studio) ![GitHub stars](https://img.shields.io/github/stars/CherryHQ/cherry-studio?style=flat&label=%E2%AD%90) - Desktop AI client with assistants and agents; works with Ollama and other providers.
- [Chatbox](https://github.com/chatboxai/chatbox) ![GitHub stars](https://img.shields.io/github/stars/chatboxai/chatbox?style=flat&label=%E2%AD%90) - Cross-platform AI client with Ollama support.
- [SillyTavern](https://github.com/SillyTavern/SillyTavern) ![GitHub stars](https://img.shields.io/github/stars/SillyTavern/SillyTavern?style=flat&label=%E2%AD%90) - LLM front-end for power users (character / role-play oriented).

---

## Local-first RAG, knowledge & agents

- [PrivateGPT](https://github.com/zylon-ai/private-gpt) ![GitHub stars](https://img.shields.io/github/stars/zylon-ai/private-gpt?style=flat&label=%E2%AD%90) - API layer for private AI apps on local models: RAG, tools, MCP, text-to-SQL.
- [Khoj](https://khoj.dev/) ![GitHub stars](https://img.shields.io/github/stars/khoj-ai/khoj?style=flat&label=%E2%AD%90) - Self-hostable AI second brain over your docs and the web; works with local LLMs. ([GitHub](https://github.com/khoj-ai/khoj))
- [Langchain-Chatchat](https://github.com/chatchat-space/Langchain-Chatchat) ![GitHub stars](https://img.shields.io/github/stars/chatchat-space/Langchain-Chatchat?style=flat&label=%E2%AD%90) - Local knowledge-base RAG and agent app (ChatGLM, Qwen, Llama; Chinese-oriented).
- [Local Deep Research](https://github.com/LearningCircuit/local-deep-research) ![GitHub stars](https://img.shields.io/github/stars/LearningCircuit/local-deep-research?style=flat&label=%E2%AD%90) - Deep-research assistant using local LLMs, multiple search engines, and private documents.
- [AgenticSeek](https://github.com/Fosowl/agenticSeek) ![GitHub stars](https://img.shields.io/github/stars/Fosowl/agenticSeek?style=flat&label=%E2%AD%90) - Fully local autonomous agent that browses, codes, and plans.
- [llmware](https://github.com/llmware-ai/llmware) ![GitHub stars](https://img.shields.io/github/stars/llmware-ai/llmware?style=flat&label=%E2%AD%90) - Framework for enterprise RAG pipelines with small, specialized models.
- [Meetily](https://github.com/Zackriya-Solutions/meetily) ![GitHub stars](https://img.shields.io/github/stars/Zackriya-Solutions/meetily?style=flat&label=%E2%AD%90) - 100% local meeting transcription and summarization (Whisper / Parakeet + Ollama).

---

## Fine-tuning

- [Unsloth](https://unsloth.ai/) ![GitHub stars](https://img.shields.io/github/stars/unslothai/unsloth?style=flat&label=%E2%AD%90) - Fast, memory-efficient fine-tuning and RL, now with a local UI to run and train models. ([GitHub](https://github.com/unslothai/unsloth))

---

## Model selection & utilities

- [whichllm](https://github.com/Andyyyy64/whichllm) ![GitHub stars](https://img.shields.io/github/stars/Andyyyy64/whichllm?style=flat&label=%E2%AD%90) - Finds the local LLM that runs and performs best on your hardware, ranked by recent benchmarks.
- [GraphicCardPrices VRAM calculator](https://graphiccardprices.com/llm-vram-estimator/) - Free browser worksheet for local LLM memory planning with adjustable weight precision, KV cache, runtime overhead and headroom. Proprietary; funded through Amazon US affiliate links. Estimates only, not benchmarks or fit guarantees.
- [Hugging Face Hub](https://huggingface.co/models) - Main source of open model weights (search for GGUF, MLX, or AWQ / GPTQ variants).

---

## Archived / inactive

Kept for reference; no longer maintained.

- [h2oGPT](https://github.com/h2oai/h2ogpt) ![GitHub stars](https://img.shields.io/github/stars/h2oai/h2ogpt?style=flat&label=%E2%AD%90) - Private document / image chat with local models (archived).
- [IPEX-LLM](https://github.com/intel/ipex-llm) ![GitHub stars](https://img.shields.io/github/stars/intel/ipex-llm?style=flat&label=%E2%AD%90) - Local LLM acceleration on Intel CPU / iGPU / NPU / Arc (archived).
- [Hugging Face TGI](https://github.com/huggingface/text-generation-inference) ![GitHub stars](https://img.shields.io/github/stars/huggingface/text-generation-inference?style=flat&label=%E2%AD%90) - Text Generation Inference server (archived).

---

## Related lists

- [rafska/awesome-local-llm](https://github.com/rafska/awesome-local-llm) ![GitHub stars](https://img.shields.io/github/stars/rafska/awesome-local-llm?style=flat&label=%E2%AD%90) - Platforms, tools, practices, and resources for running LLMs locally.
- [janhq/awesome-local-ai](https://github.com/janhq/awesome-local-ai) ![GitHub stars](https://img.shields.io/github/stars/janhq/awesome-local-ai?style=flat&label=%E2%AD%90) - Local AI tools curated by the Jan team.
- [vince-lam/awesome-local-llms](https://github.com/vince-lam/awesome-local-llms) ![GitHub stars](https://img.shields.io/github/stars/vince-lam/awesome-local-llms?style=flat&label=%E2%AD%90) - Compares local LLM projects by popularity and activity metrics.
- [Hannibal046/Awesome-LLM](https://github.com/Hannibal046/Awesome-LLM) ![GitHub stars](https://img.shields.io/github/stars/Hannibal046/Awesome-LLM?style=flat&label=%E2%AD%90) - General LLM resources.
- [tensorchord/Awesome-LLMOps](https://github.com/tensorchord/Awesome-LLMOps) ![GitHub stars](https://img.shields.io/github/stars/tensorchord/Awesome-LLMOps?style=flat&label=%E2%AD%90) - LLMOps and serving tools.
- [xlite-dev/Awesome-LLM-Inference](https://github.com/xlite-dev/Awesome-LLM-Inference) ![GitHub stars](https://img.shields.io/github/stars/xlite-dev/Awesome-LLM-Inference?style=flat&label=%E2%AD%90) - LLM inference papers with code.
- [awesome-selfhosted/awesome-selfhosted](https://github.com/awesome-selfhosted/awesome-selfhosted) ![GitHub stars](https://img.shields.io/github/stars/awesome-selfhosted/awesome-selfhosted?style=flat&label=%E2%AD%90) - Self-hosted software in general.
- [sindresorhus/awesome](https://github.com/sindresorhus/awesome) ![GitHub stars](https://img.shields.io/github/stars/sindresorhus/awesome?style=flat&label=%E2%AD%90) - The Awesome meta-list.

---

## Contributing

Contributions welcome — open a pull request to add a resource, fix a broken link, or suggest a category.

Prefer **durable official / project URLs**, short blurbs, and actively maintained open-source projects. Add a ⭐ star badge for GitHub projects, and note when an app is closed source or a project is archived. Update both `README.md` and `README.ja.md` when you can.
