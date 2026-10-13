# Awesome Local LLM（日本語）

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

[English README](README.md)

**ローカル LLM** 向けの有用なリソースの厳選リストです。推論エンジン、デスクトップアプリ・チャット UI、ローカルファーストな RAG／エージェント、ファインチューニング、手元のハードに合うモデル選びのツールなどをまとめています。できるだけ公式／プロジェクトの耐久性のある URL を優先しています。

**発見・学習用のリストです。** ベンチマークやランキングではありません。ダウンロード前に各モデルのライセンスと、自分のハードウェア（VRAM／メモリ）を確認してください。⭐ バッジは GitHub のスター数をリアルタイム表示します（shields.io）。

## 目次

- [推論エンジン・ランタイム](#推論エンジンランタイム)
- [サービングフレームワーク（GPU／サーバー）](#サービングフレームワークgpuサーバー)
- [Apple Silicon・エッジ・特殊ハードウェア](#apple-siliconエッジ特殊ハードウェア)
- [デスクトップアプリ](#デスクトップアプリ)
- [チャット UI・フロントエンド](#チャット-uiフロントエンド)
- [ローカルファーストな RAG・ナレッジ・エージェント](#ローカルファーストな-ragナレッジエージェント)
- [ファインチューニング](#ファインチューニング)
- [モデル選び・ユーティリティ](#モデル選びユーティリティ)
- [アーカイブ済み・停止中](#アーカイブ済み停止中)
- [関連リスト](#関連リスト)
- [コントリビューション](#コントリビューション)

---

## 推論エンジン・ランタイム

自分の PC（CPU や一般向け GPU）でモデルを動かすためのもの。

- [Ollama（英語）](https://ollama.com/) ![GitHub stars](https://img.shields.io/github/stars/ollama/ollama?style=flat&label=%E2%AD%90) - コマンド1つでオープンモデルを取得・実行できる定番ツール。ローカル REST API 付き。（[GitHub](https://github.com/ollama/ollama)）
- [llama.cpp（英語）](https://github.com/ggml-org/llama.cpp) ![GitHub stars](https://img.shields.io/github/stars/ggml-org/llama.cpp?style=flat&label=%E2%AD%90) - C/C++ 製の LLM 推論エンジン。GGUF 形式の本家で、多くのツールの土台。
- [LocalAI（英語）](https://localai.io/) ![GitHub stars](https://img.shields.io/github/stars/mudler/LocalAI?style=flat&label=%E2%AD%90) - LLM・画像認識・音声・画像生成・動画に対応した OpenAI 互換 API サーバー。GPU なしでも動作。（[GitHub](https://github.com/mudler/LocalAI)）
- [llamafile（英語）](https://github.com/mozilla-ai/llamafile) ![GitHub stars](https://img.shields.io/github/stars/mozilla-ai/llamafile?style=flat&label=%E2%AD%90) - LLM を OS をまたいで動く単一の実行ファイルとして配布・実行（Mozilla.ai）。
- [Xinference（英語）](https://github.com/xorbitsai/inference) ![GitHub stars](https://img.shields.io/github/stars/xorbitsai/inference?style=flat&label=%E2%AD%90) - llama.cpp・vLLM・SGLang・transformers などを OpenAI 互換の統一 API で扱える推論基盤。
- [PowerInfer（英語）](https://github.com/Tiiny-AI/PowerInfer) ![GitHub stars](https://img.shields.io/github/stars/Tiiny-AI/PowerInfer?style=flat&label=%E2%AD%90) - 一般向け GPU でのローカル実行に特化した高速推論。
- [ExLlamaV2（英語）](https://github.com/turboderp-org/exllamav2) ![GitHub stars](https://img.shields.io/github/stars/turboderp-org/exllamav2?style=flat&label=%E2%AD%90) - 最近の一般向け GPU で LLM を高速に動かす推論ライブラリ。

---

## サービングフレームワーク（GPU／サーバー）

ワークステーションや社内サーバー向けの高スループットなエンジン。

- [vLLM（英語）](https://docs.vllm.ai/) ![GitHub stars](https://img.shields.io/github/stars/vllm-project/vllm?style=flat&label=%E2%AD%90) - 高スループットでメモリ効率の良い推論・配信エンジン。（[GitHub](https://github.com/vllm-project/vllm)）
- [SGLang（英語）](https://github.com/sgl-project/sglang) ![GitHub stars](https://img.shields.io/github/stars/sgl-project/sglang?style=flat&label=%E2%AD%90) - LLM・マルチモーダルモデル向けの高性能サービングフレームワーク。
- [LMDeploy（英語）](https://github.com/InternLM/lmdeploy) ![GitHub stars](https://img.shields.io/github/stars/InternLM/lmdeploy?style=flat&label=%E2%AD%90) - LLM の圧縮・デプロイ・配信ツールキット（TurboMind エンジン）。

---

## Apple Silicon・エッジ・特殊ハードウェア

- [MLX（英語）](https://github.com/ml-explore/mlx) ![GitHub stars](https://img.shields.io/github/stars/ml-explore/mlx?style=flat&label=%E2%AD%90) - Apple による Apple Silicon 向け計算フレームワーク。（LLM の実行は [mlx-lm](https://github.com/ml-explore/mlx-lm) ![GitHub stars](https://img.shields.io/github/stars/ml-explore/mlx-lm?style=flat&label=%E2%AD%90)）
- [MLC LLM（英語）](https://llm.mlc.ai/) ![GitHub stars](https://img.shields.io/github/stars/mlc-ai/mlc-llm?style=flat&label=%E2%AD%90) - 機械学習コンパイルでスマホ・ブラウザ・GPU などへ展開できる汎用エンジン。（[GitHub](https://github.com/mlc-ai/mlc-llm)）
- [exo（英語）](https://github.com/exo-explore/exo) ![GitHub stars](https://img.shields.io/github/stars/exo-explore/exo?style=flat&label=%E2%AD%90) - 手持ちの複数デバイスをつないで大きなモデルを分散実行。
- [BitNet（英語）](https://github.com/microsoft/BitNet) ![GitHub stars](https://img.shields.io/github/stars/microsoft/BitNet?style=flat&label=%E2%AD%90) - Microsoft 公式の 1ビット LLM 推論フレームワーク（CPU でも軽快）。
- [Lemonade（英語）](https://github.com/lemonade-sdk/lemonade) ![GitHub stars](https://img.shields.io/github/stars/lemonade-sdk/lemonade?style=flat&label=%E2%AD%90) - AMD の GPU／NPU（Ryzen AI、Radeon。ROCm／Vulkan／ONNX）向けに最適化したローカル LLM サーバー。

---

## デスクトップアプリ

モデルのダウンロードからオフラインでのチャットまで完結するアプリ。

- [LM Studio（英語）](https://lmstudio.ai/) - ローカルモデルを探して実行できる人気のデスクトップアプリ（本体はクローズドソース。[lms CLI](https://github.com/lmstudio-ai/lms) ![GitHub stars](https://img.shields.io/github/stars/lmstudio-ai/lms?style=flat&label=%E2%AD%90) はオープンソース）。
- [Jan（英語）](https://jan.ai/) ![GitHub stars](https://img.shields.io/github/stars/janhq/jan?style=flat&label=%E2%AD%90) - 完全オフラインで動く、オープンソースの ChatGPT 代替。（[GitHub](https://github.com/janhq/jan)）
- [GPT4All（英語）](https://www.nomic.ai/gpt4all) ![GitHub stars](https://img.shields.io/github/stars/nomic-ai/gpt4all?style=flat&label=%E2%AD%90) - どの端末でもローカル LLM を動かせるアプリ（Nomic）。（[GitHub](https://github.com/nomic-ai/gpt4all)）
- [textgen（旧 text-generation-webui）（英語）](https://github.com/oobabooga/textgen) ![GitHub stars](https://img.shields.io/github/stars/oobabooga/textgen?style=flat&label=%E2%AD%90) - ローカル LLM 用のオープンソースデスクトップアプリ。OpenAI／Anthropic 互換 API 付き。
- [AnythingLLM（英語）](https://anythingllm.com/) ![GitHub stars](https://img.shields.io/github/stars/Mintplex-Labs/anything-llm?style=flat&label=%E2%AD%90) - RAG とエージェント機能を備えたローカルファーストのデスクトップ／セルフホストアプリ。（[GitHub](https://github.com/Mintplex-Labs/anything-llm)）

---

## チャット UI・フロントエンド

Ollama、llama.cpp、各種 OpenAI 互換エンドポイントにつないで使う画面。

- [Open WebUI（英語）](https://openwebui.com/) ![GitHub stars](https://img.shields.io/github/stars/open-webui/open-webui?style=flat&label=%E2%AD%90) - Ollama や OpenAI 互換 API 向けの高機能なセルフホスト Web UI（RAG、MCP 対応）。（[GitHub](https://github.com/open-webui/open-webui)）
- [LobeHub（英語）](https://github.com/lobehub/lobehub) ![GitHub stars](https://img.shields.io/github/stars/lobehub/lobehub?style=flat&label=%E2%AD%90) - ローカル／クラウド両対応のエージェントワークスペース兼チャット UI（旧 Lobe Chat）。
- [Cherry Studio（英語）](https://github.com/CherryHQ/cherry-studio) ![GitHub stars](https://img.shields.io/github/stars/CherryHQ/cherry-studio?style=flat&label=%E2%AD%90) - アシスタントやエージェント機能を備えたデスクトップ AI クライアント。Ollama などに対応。
- [Chatbox（英語）](https://github.com/chatboxai/chatbox) ![GitHub stars](https://img.shields.io/github/stars/chatboxai/chatbox?style=flat&label=%E2%AD%90) - Ollama に対応したクロスプラットフォームの AI クライアント。
- [SillyTavern（英語）](https://github.com/SillyTavern/SillyTavern) ![GitHub stars](https://img.shields.io/github/stars/SillyTavern/SillyTavern?style=flat&label=%E2%AD%90) - 上級者向けの LLM フロントエンド（キャラクター／ロールプレイ向け）。

---

## ローカルファーストな RAG・ナレッジ・エージェント

- [PrivateGPT（英語）](https://github.com/zylon-ai/private-gpt) ![GitHub stars](https://img.shields.io/github/stars/zylon-ai/private-gpt?style=flat&label=%E2%AD%90) - ローカルモデルでプライベート AI アプリを作るための API 基盤（RAG、ツール、MCP、Text-to-SQL）。
- [Khoj（英語）](https://khoj.dev/) ![GitHub stars](https://img.shields.io/github/stars/khoj-ai/khoj?style=flat&label=%E2%AD%90) - 手元の文書や Web をもとに答えるセルフホスト可能な「AI セカンドブレイン」。ローカル LLM にも対応。（[GitHub](https://github.com/khoj-ai/khoj)）
- [Langchain-Chatchat（中国語／英語）](https://github.com/chatchat-space/Langchain-Chatchat) ![GitHub stars](https://img.shields.io/github/stars/chatchat-space/Langchain-Chatchat?style=flat&label=%E2%AD%90) - ローカルナレッジベースの RAG／エージェントアプリ（ChatGLM、Qwen、Llama。中国語圏向け）。
- [Local Deep Research（英語）](https://github.com/LearningCircuit/local-deep-research) ![GitHub stars](https://img.shields.io/github/stars/LearningCircuit/local-deep-research?style=flat&label=%E2%AD%90) - ローカル LLM・複数の検索エンジン・手元の文書を使うディープリサーチツール。
- [AgenticSeek（英語）](https://github.com/Fosowl/agenticSeek) ![GitHub stars](https://img.shields.io/github/stars/Fosowl/agenticSeek?style=flat&label=%E2%AD%90) - Web 閲覧・コーディング・計画を行う完全ローカルの自律エージェント。
- [llmware（英語）](https://github.com/llmware-ai/llmware) ![GitHub stars](https://img.shields.io/github/stars/llmware-ai/llmware?style=flat&label=%E2%AD%90) - 小型の特化モデルで企業向け RAG パイプラインを作るフレームワーク。
- [Meetily（英語）](https://github.com/Zackriya-Solutions/meetily) ![GitHub stars](https://img.shields.io/github/stars/Zackriya-Solutions/meetily?style=flat&label=%E2%AD%90) - 完全ローカルの会議文字起こし・要約（Whisper／Parakeet＋Ollama）。

---

## ファインチューニング

- [Unsloth（英語）](https://unsloth.ai/) ![GitHub stars](https://img.shields.io/github/stars/unslothai/unsloth?style=flat&label=%E2%AD%90) - 高速・省メモリなファインチューニングと強化学習。モデルの実行・学習ができるローカル UI も提供。（[GitHub](https://github.com/unslothai/unsloth)）

---

## モデル選び・ユーティリティ

- [whichllm（英語）](https://github.com/Andyyyy64/whichllm) ![GitHub stars](https://img.shields.io/github/stars/Andyyyy64/whichllm?style=flat&label=%E2%AD%90) - 手元のハードで動き、最も性能が出るローカル LLM を最新ベンチマークで選んでくれるツール。
- [Hugging Face Hub（英語）](https://huggingface.co/models) - オープンモデルの主な入手先（GGUF、MLX、AWQ／GPTQ 版などで検索）。
- [LocalForge（英語）](https://localai.hexmobius.com/en?utm_source=github&utm_medium=awesome_list&utm_campaign=shvyac_awesome_local_llm) - ローカルモデルやマシンを選ぶための意思決定リファレンス。メモリ適合、実用コンテキスト、第三者が実測した速度（量子化・ランタイム・同時実行数つき）、不明点を分けて示し、デプロイ用コマンドを提示します。自前の検証機は持たず、独自の速度値も公開しません。

---

## アーカイブ済み・停止中

参考として残しています。メンテナンスは終了しています。

- [h2oGPT（英語）](https://github.com/h2oai/h2ogpt) ![GitHub stars](https://img.shields.io/github/stars/h2oai/h2ogpt?style=flat&label=%E2%AD%90) - ローカルモデルで文書や画像とチャットできるツール（アーカイブ済み）。
- [IPEX-LLM（英語）](https://github.com/intel/ipex-llm) ![GitHub stars](https://img.shields.io/github/stars/intel/ipex-llm?style=flat&label=%E2%AD%90) - Intel の CPU／内蔵 GPU／NPU／Arc 向けローカル LLM 高速化（アーカイブ済み）。
- [Hugging Face TGI（英語）](https://github.com/huggingface/text-generation-inference) ![GitHub stars](https://img.shields.io/github/stars/huggingface/text-generation-inference?style=flat&label=%E2%AD%90) - Text Generation Inference サーバー（アーカイブ済み）。

---

## 関連リスト

- [rafska/awesome-local-llm（英語）](https://github.com/rafska/awesome-local-llm) ![GitHub stars](https://img.shields.io/github/stars/rafska/awesome-local-llm?style=flat&label=%E2%AD%90) - LLM をローカルで動かすための基盤・ツール・実践・リソース集。
- [janhq/awesome-local-ai（英語）](https://github.com/janhq/awesome-local-ai) ![GitHub stars](https://img.shields.io/github/stars/janhq/awesome-local-ai?style=flat&label=%E2%AD%90) - Jan チームによるローカル AI ツール集。
- [vince-lam/awesome-local-llms（英語）](https://github.com/vince-lam/awesome-local-llms) ![GitHub stars](https://img.shields.io/github/stars/vince-lam/awesome-local-llms?style=flat&label=%E2%AD%90) - ローカル LLM プロジェクトを人気度・活発さの指標で比較。
- [Hannibal046/Awesome-LLM（英語）](https://github.com/Hannibal046/Awesome-LLM) ![GitHub stars](https://img.shields.io/github/stars/Hannibal046/Awesome-LLM?style=flat&label=%E2%AD%90) - LLM 全般のリソース。
- [tensorchord/Awesome-LLMOps（英語）](https://github.com/tensorchord/Awesome-LLMOps) ![GitHub stars](https://img.shields.io/github/stars/tensorchord/Awesome-LLMOps?style=flat&label=%E2%AD%90) - LLMOps・配信ツール。
- [xlite-dev/Awesome-LLM-Inference（英語）](https://github.com/xlite-dev/Awesome-LLM-Inference) ![GitHub stars](https://img.shields.io/github/stars/xlite-dev/Awesome-LLM-Inference?style=flat&label=%E2%AD%90) - LLM 推論の論文とコード。
- [awesome-selfhosted/awesome-selfhosted（英語）](https://github.com/awesome-selfhosted/awesome-selfhosted) ![GitHub stars](https://img.shields.io/github/stars/awesome-selfhosted/awesome-selfhosted?style=flat&label=%E2%AD%90) - セルフホスト用ソフト全般。
- [sindresorhus/awesome（英語）](https://github.com/sindresorhus/awesome) ![GitHub stars](https://img.shields.io/github/stars/sindresorhus/awesome?style=flat&label=%E2%AD%90) - Awesome のメタリスト。

---

## コントリビューション

コントリビューション歓迎です。リソース追加、リンク切れ修正、カテゴリ提案はプルリクエストでどうぞ。

**公式／プロジェクトの耐久性のある URL**、短い説明、継続的にメンテナンスされているオープンソースプロジェクトを優先してください。GitHub のプロジェクトには ⭐ スター数バッジを付け、クローズドソースのアプリやアーカイブ済みのプロジェクトはその旨を明記してください。可能なら `README.md` と `README.ja.md` の両方を更新してください。
