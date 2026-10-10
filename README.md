# Awesome Local LLM

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

[日本語版はこちら / Japanese](README.ja.md)

A curated list of useful **local LLM** resources — inference engines, desktop apps and chat UIs, local-first RAG / agents, fine-tuning, and tools for picking a model that fits your hardware. Prefer durable official / project URLs.

**Discovery list only** — not a benchmark or ranking. Check each model's license and your hardware (VRAM / RAM) before downloading.

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

- [Ollama](https://ollama.com/) - The most popular way to pull and run open models with one command; local REST API. ([GitHub](https://github.com/ollama/ollama))
- [llama.cpp](https://github.com/ggml-org/llama.cpp) - LLM inference in C/C++; home of the GGUF format and the engine behind many other tools.
- [LocalAI](https://localai.io/) - OpenAI-compatible API server for LLMs, vision, voice, image, and video; no GPU required. ([GitHub](https://github.com/mudler/LocalAI))
- [llamafile](https://github.com/mozilla-ai/llamafile) - Distribute and run an LLM as a single cross-platform executable (Mozilla.ai).
- [Xinference](https://github.com/xorbitsai/inference) - Unified, OpenAI-compatible inference API across llama.cpp, vLLM, SGLang, transformers, and more.
- [PowerInfer](https://github.com/Tiiny-AI/PowerInfer) - High-speed LLM serving for local deployment on consumer GPUs.
- [ExLlamaV2](https://github.com/turboderp-org/exllamav2) - Fast inference library for running LLMs on modern consumer GPUs.

---

## Serving frameworks (GPU / server)

High-throughput engines for a workstation or on-prem server.

- [vLLM](https://docs.vllm.ai/) - High-throughput, memory-efficient inference and serving engine. ([GitHub](https://github.com/vllm-project/vllm))
- [SGLang](https://github.com/sgl-project/sglang) - High-performance serving framework for LLMs and multimodal models.
- [LMDeploy](https://github.com/InternLM/lmdeploy) - Toolkit for compressing, deploying, and serving LLMs (TurboMind engine).

---

## Apple Silicon, edge & special hardware

- [MLX](https://github.com/ml-explore/mlx) - Apple's array framework for Apple silicon. ([mlx-lm](https://github.com/ml-explore/mlx-lm) for running LLMs)
- [MLC LLM](https://llm.mlc.ai/) - Universal deployment engine with ML compilation (phones, browsers, GPUs). ([GitHub](https://github.com/mlc-ai/mlc-llm))
- [exo](https://github.com/exo-explore/exo) - Run large models across a cluster of your own devices.
- [BitNet](https://github.com/microsoft/BitNet) - Microsoft's official inference framework for 1-bit LLMs (CPU-friendly).
- [Lemonade](https://github.com/lemonade-sdk/lemonade) - Local LLM server optimized for AMD GPUs and NPUs (Ryzen AI, Radeon; ROCm / Vulkan / ONNX).

---

## Desktop apps

All-in-one apps for downloading models and chatting offline.

- [LM Studio](https://lmstudio.ai/) - Popular desktop app for discovering and running local models (app is closed source; [lms CLI](https://github.com/lmstudio-ai/lms) is open source).
- [Jan](https://jan.ai/) - Open-source ChatGPT alternative that runs 100% offline. ([GitHub](https://github.com/janhq/jan))
- [GPT4All](https://www.nomic.ai/gpt4all) - Run local LLMs on any device (Nomic). ([GitHub](https://github.com/nomic-ai/gpt4all))
- [textgen (formerly text-generation-webui)](https://github.com/oobabooga/textgen) - Open-source desktop app for local LLMs with OpenAI / Anthropic-compatible API.
- [AnythingLLM](https://anythingllm.com/) - Local-first desktop / self-hosted app with RAG and agents. ([GitHub](https://github.com/Mintplex-Labs/anything-llm))

---

## Chat UIs & front-ends

Connect to Ollama, llama.cpp, or any OpenAI-compatible endpoint.

- [Open WebUI](https://openwebui.com/) - Feature-rich self-hosted web UI for Ollama and OpenAI-compatible APIs (RAG, MCP). ([GitHub](https://github.com/open-webui/open-webui))
- [LobeHub](https://github.com/lobehub/lobehub) - Agent workspace / chat UI (formerly Lobe Chat) supporting local and cloud models.
- [Cherry Studio](https://github.com/CherryHQ/cherry-studio) - Desktop AI client with assistants and agents; works with Ollama and other providers.
- [Chatbox](https://github.com/chatboxai/chatbox) - Cross-platform AI client with Ollama support.
- [SillyTavern](https://github.com/SillyTavern/SillyTavern) - LLM front-end for power users (character / role-play oriented).

---

## Local-first RAG, knowledge & agents

- [PrivateGPT](https://github.com/zylon-ai/private-gpt) - API layer for private AI apps on local models: RAG, tools, MCP, text-to-SQL.
- [Khoj](https://khoj.dev/) - Self-hostable AI second brain over your docs and the web; works with local LLMs. ([GitHub](https://github.com/khoj-ai/khoj))
- [Langchain-Chatchat](https://github.com/chatchat-space/Langchain-Chatchat) - Local knowledge-base RAG and agent app (ChatGLM, Qwen, Llama; Chinese-oriented).
- [Local Deep Research](https://github.com/LearningCircuit/local-deep-research) - Deep-research assistant using local LLMs, multiple search engines, and private documents.
- [AgenticSeek](https://github.com/Fosowl/agenticSeek) - Fully local autonomous agent that browses, codes, and plans.
- [llmware](https://github.com/llmware-ai/llmware) - Framework for enterprise RAG pipelines with small, specialized models.
- [Meetily](https://github.com/Zackriya-Solutions/meetily) - 100% local meeting transcription and summarization (Whisper / Parakeet + Ollama).

---

## Fine-tuning

- [Unsloth](https://unsloth.ai/) - Fast, memory-efficient fine-tuning and RL, now with a local UI to run and train models. ([GitHub](https://github.com/unslothai/unsloth))

---

## Model selection & utilities

- [whichllm](https://github.com/Andyyyy64/whichllm) - Finds the local LLM that runs and performs best on your hardware, ranked by recent benchmarks.
- [Hugging Face Hub](https://huggingface.co/models) - Main source of open model weights (search for GGUF, MLX, or AWQ / GPTQ variants).

---

## Archived / inactive

Kept for reference; no longer maintained.

- [h2oGPT](https://github.com/h2oai/h2ogpt) - Private document / image chat with local models (archived).
- [IPEX-LLM](https://github.com/intel/ipex-llm) - Local LLM acceleration on Intel CPU / iGPU / NPU / Arc (archived).
- [Hugging Face TGI](https://github.com/huggingface/text-generation-inference) - Text Generation Inference server (archived).

---

## Related lists

- [rafska/awesome-local-llm](https://github.com/rafska/awesome-local-llm) - Platforms, tools, practices, and resources for running LLMs locally.
- [janhq/awesome-local-ai](https://github.com/janhq/awesome-local-ai) - Local AI tools curated by the Jan team.
- [vince-lam/awesome-local-llms](https://github.com/vince-lam/awesome-local-llms) - Compares local LLM projects by popularity and activity metrics.
- [Hannibal046/Awesome-LLM](https://github.com/Hannibal046/Awesome-LLM) - General LLM resources.
- [tensorchord/Awesome-LLMOps](https://github.com/tensorchord/Awesome-LLMOps) - LLMOps and serving tools.
- [xlite-dev/Awesome-LLM-Inference](https://github.com/xlite-dev/Awesome-LLM-Inference) - LLM inference papers with code.
- [awesome-selfhosted/awesome-selfhosted](https://github.com/awesome-selfhosted/awesome-selfhosted) - Self-hosted software in general.
- [sindresorhus/awesome](https://github.com/sindresorhus/awesome) - The Awesome meta-list.

---

## Contributing

Contributions welcome — open a pull request to add a resource, fix a broken link, or suggest a category.

Prefer **durable official / project URLs**, short blurbs, and actively maintained open-source projects. Note when an app is closed source or a project is archived. Update both `README.md` and `README.ja.md` when you can.
