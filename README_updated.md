# <p align="center">Awesome-Weather-Forecast</p>

<div align="center">

![GitHub stars](https://img.shields.io/github/stars/zhengkai15/Awesome-Weather-Forecast.svg?color=red&style=for-the-badge)
![GitHub forks](https://img.shields.io/github/forks/zhengkai15/Awesome-Weather-Forecast.svg?style=for-the-badge)
![GitHub activity](https://img.shields.io/github/last-commit/zhengkai15/Awesome-Weather-Forecast?color=yellow&style=for-the-badge)
![GitHub issues](https://img.shields.io/github/issues/zhengkai15/Awesome-Weather-Forecast?style=for-the-badge)
![GitHub closed issues](https://img.shields.io/github/issues-closed/zhengkai15/Awesome-Weather-Forecast?color=inactive&style=for-the-badge)

[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)
[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fzhengkai15%2FAwesome-Weather-Forecast&count_bg=%23DD4B78&title_bg=%23555555&icon=jabber.svg&icon_color=%23E7E7E7&title=Hits(2024.02~)&edge_flat=false)](https://hits.seeyoufarm.com)
[![Star History Chart](https://api.star-history.com/svg?repos=zhengkai15/Awesome-Weather-Forecast&type=Date)](https://star-history.com/#zhengkai15/Awesome-Weather-Forecast&Date)

</div>

A curated list of papers and resources on **AI-driven weather forecasting**, covering deep learning, generative models, foundation models, LLMs, and agents across the full forecasting pipeline — from data assimilation to sub-seasonal prediction.

> **Keywords:** AI weather forecast · deep learning meteorology · NWP · diffusion model · foundation model · nowcasting · data assimilation · LLM climate · atmospheric AI · neural weather model

> **Want to contribute?** See [CONTRIBUTING.md](./CONTRIBUTING.md) · Submit via [Issues](https://github.com/zhengkai15/Awesome-Weather-Forecast/issues/new/choose) or PR · Maintained by [@zhengkai15](https://zhengkai15.github.io/)

> ⭐ **Star this repo** to stay updated with the latest AI weather papers!

---

## 📋 Table of Contents

| # | Category | Description |
|---|---|---|
| 1 | [🌍 Medium-Range Forecast](#-1-medium-range-forecast-115-days) | Global/regional 1–15 day deterministic & ensemble forecast |
| 2 | [⚡ NowCasting](#-2-nowcasting-06-hours) | 0–6 hour precipitation & radar echo extrapolation |
| 3 | [🔬 Super Resolution / Downscaling](#-3-super-resolution--downscaling) | Spatial downscaling from NWP/climate model outputs |
| 4 | [🔄 Data Assimilation](#-4-data-assimilation) | ML-based initial condition estimation |
| 5 | [🌪️ Extreme Weather](#%EF%B8%8F-5-extreme-weather-incl-typhoon) | High-impact events including typhoon/tropical cyclone |
| 6 | [🌡️ Seasonal & Climate](#%EF%B8%8F-6-seasonal--climate-forecast) | Sub-seasonal to seasonal (S2S) and climate simulation |
| 7 | [🗜️ Data Compression](#%EF%B8%8F-7-weather-data-compression) | Compact latent representations for ERA5/CMIP6 |
| 8 | [🏗️ Foundation Models](#%EF%B8%8F-8-atmospheric-foundation-models) | Large pre-trained multi-task atmospheric models |
| 9 | [🤖 LLM / Agent / Multimodal](#-9-llm-agent--multimodal-weather) | LLMs, agents, and multimodal models for weather science |
| 10 | [🤖 AI Auto-Research](#-10-ai-auto-research) | AI-driven scientific discovery workflows and research agents |
---

## 🗓️ Latest Updates

| Date | Update |
|---|---|
| 2026-08 | Added AI auto research |
| 2026-07 | Refactored into categorized `papers/` structure; added 29 new papers (2024–2026) |
| 2025-08 | Added AlphaPre (CVPR 2025), FuXi-Regional, CRA5 |
| 2024-02 | Initial release with Medium-Range, NowCasting, SR, DA categories |

---

## 🌍 1. Medium-Range Forecast (1–15 Days)

→ **[Full list](./papers/01_medium_range.md)**

**Highlights:** Pangu · GraphCast · FuXi · FengWu · Aurora · GenCast · NeuralGCM · AIFS · Stormer · FuXi-ENS · SEEDS

<details>
<summary>Preview (click to expand)</summary>

| Model | Venue | Core Contribution |
|---|---|---|
| [Pangu-Weather](./papers/01_medium_range.md) | Nature 2023 | 3D Earth-specific transformer |
| [GraphCast](./papers/01_medium_range.md) | Science 2023 | GNN surpassing ECMWF HRES |
| [Aurora](./papers/01_medium_range.md) | Nature 2025 | 1.3B-param foundation model |
| [NeuralGCM](./papers/01_medium_range.md) | Nature 2024 | Hybrid physics+ML GCM |
| [AIFS](./papers/01_medium_range.md) | ECMWF 2024 | First operational ML NWP |
| [GenCast](./papers/01_medium_range.md) | Nature 2024 | Diffusion ensemble forecast |

</details>

---

## ⚡ 2. NowCasting (0–6 Hours)

→ **[Full list](./papers/02_nowcasting.md)**

**Highlights:** NowcastNet · PreDiff · AlphaPre · DiffCast · CasCast · WoFSCast · StormCast

<details>
<summary>Preview (click to expand)</summary>

| Model | Venue | Core Contribution |
|---|---|---|
| [NowcastNet](./papers/02_nowcasting.md) | Nature 2023 | Physics-constrained GAN |
| [PreDiff](./papers/02_nowcasting.md) | NeurIPS 2023 | Latent diffusion nowcasting |
| [AlphaPre](./papers/02_nowcasting.md) | CVPR 2025 | Amplitude-phase disentanglement |
| [DiffCast](./papers/02_nowcasting.md) | CVPR 2024 | Deterministic+stochastic diffusion |
| [CasCast](./papers/02_nowcasting.md) | ICML 2024 | Cascaded extreme precip |
| [WoFSCast](./papers/02_nowcasting.md) | GRL 2025 | Warning-scale convective ML |

</details>

---

## 🔬 3. Super Resolution / Downscaling

→ **[Full list](./papers/03_super_resolution.md)**

**Highlights:** CorrDiff · FengWu-GHR · STVD · StormCast · DeepSD · SRDRN

<details>
<summary>Preview (click to expand)</summary>

| Model | Venue | Core Contribution |
|---|---|---|
| [CorrDiff](./papers/03_super_resolution.md) | arXiv 2023 | NVIDIA residual diffusion 25km→2km |
| [STVD](./papers/03_super_resolution.md) | NeurIPS 2024 | Spatiotemporal video diffusion SR |
| [FengWu-GHR](./papers/03_super_resolution.md) | arXiv 2024 | Km-scale global medium-range |

</details>

---

## 🔄 4. Data Assimilation

→ **[Full list](./papers/04_data_assimilation.md)**

**Highlights:** FuXi-DA · FengWu-4DVar · DiffDA · Score-based DA · LDA

<details>
<summary>Preview (click to expand)</summary>

| Model | Venue | Core Contribution |
|---|---|---|
| [DiffDA](./papers/04_data_assimilation.md) | ICML 2024 | Diffusion-based sparse obs DA |
| [LDA](./papers/04_data_assimilation.md) | Science Advances 2026 | Latent space variational DA |
| [FengWu-4DVar](./papers/04_data_assimilation.md) | arXiv 2023 | ML + 4D-Var coupling |

</details>

---

## 🌪️ 5. Extreme Weather (incl. Typhoon)

→ **[Full list](./papers/05_extreme_weather.md)**

**Highlights:** FuXi-Extreme · ExtremeCast · WoFSCast · StormCast · MSCAR · AIWP-TC

<details>
<summary>Preview (click to expand)</summary>

| Model | Venue | Core Contribution |
|---|---|---|
| [FuXi-Extreme](./papers/05_extreme_weather.md) | arXiv 2023 | Extreme rainfall+wind diffusion |
| [ExtremeCast](./papers/05_extreme_weather.md) | arXiv 2024 | Asymmetric Exloss for extremes |
| [MSCAR](./papers/05_extreme_weather.md) | arXiv 2024 | Multi-modal TC intensity forecast |

</details>

---

## 🌡️ 6. Seasonal & Climate Forecast

→ **[Full list](./papers/06_seasonal_climate.md)**

**Highlights:** FuXi-S2S · NeuralGCM · ENSO-PhyNet · SEEDS · S2S-DL

<details>
<summary>Preview (click to expand)</summary>

| Model | Venue | Core Contribution |
|---|---|---|
| [FuXi-S2S](./papers/06_seasonal_climate.md) | Nat. Comm. 2024 | 42-day global ML forecast |
| [NeuralGCM](./papers/06_seasonal_climate.md) | Nature 2024 | Climate simulation hybrid GCM |
| [ENSO-PhyNet](./papers/06_seasonal_climate.md) | npj 2024 | 22-month ENSO skill |

</details>

---

## 🗜️ 7. Weather Data Compression

→ **[Full list](./papers/07_compression.md)**

**Highlights:** CRA5 · FuXi-Regional · WLA

| Model | Venue | Compression |
|---|---|---|
| [CRA5](./papers/07_compression.md) | arXiv 2024 | 226 TB → 0.7 TB (>300:1) |
| [WLA](./papers/07_compression.md) | arXiv 2025 | 244 TB → 0.43 TB |
| [FuXi-Regional](./papers/07_compression.md) | arXiv 2024 | Latent encoding for regional downscaling |

---

## 🏗️ 8. Atmospheric Foundation Models

→ **[Full list](./papers/08_foundation_models.md)**

**Highlights:** ClimaX · Aurora · Prithvi WxC · ESFM · WIND · Omni-Weather

<details>
<summary>Preview (click to expand)</summary>

| Model | Venue | Core Contribution |
|---|---|---|
| [Aurora](./papers/08_foundation_models.md) | Nature 2025 | 1.3B Microsoft atmos. foundation model |
| [Prithvi WxC](./papers/08_foundation_models.md) | ICLR 2025 Workshop | IBM/NASA 2.3B, 160 variables |
| [WIND](./papers/08_foundation_models.md) | arXiv 2026 | Zero-shot video diffusion prior |
| [ESFM](./papers/08_foundation_models.md) | arXiv 2025 | Heterogeneous earth system FM |

</details>

---

## 🤖 9. LLM, Agent & Multimodal Weather

→ **[Full list](./papers/09_llm_agent_multimodal.md)**

**Highlights:** WeatherBench 2 · ClimSim · Omni-Weather · Zephyrus · AgentCaster · WeatherQA · Weather-R1 · ClimateChat

<details>
<summary>Preview (click to expand)</summary>

| Model | Venue | Core Contribution |
|---|---|---|
| [WeatherBench 2](./papers/09_llm_agent_multimodal.md) | JAMES 2024 | Standard AI forecast evaluation vs ECMWF |
| [ClimSim](./papers/09_llm_agent_multimodal.md) | NeurIPS 2023 Best Paper | 5.7B-sample ML parameterization dataset |
| [Omni-Weather](./papers/09_llm_agent_multimodal.md) | arXiv 2025 | Multimodal radar generation + understanding |
| [Zephyrus](./papers/09_llm_agent_multimodal.md) | arXiv 2025 | Tool-calling meteorology science agent |
| [Weather-R1](./papers/09_llm_agent_multimodal.md) | ICASSP 2026 | RL-tuned multimodal reasoning VLM |

</details>

---
## 🤖 10. AI Auto-Research

→ **[Full list](./papers/10_auto_research.md)**

**Highlights:** The AI Scientist · TianJi · Zephyrus · AI Scientist-v2 · Robin · PANGAEA GPT · AutoMF

<details>
<summary>Preview (click to expand)</summary>

| Model | Venue | Core Contribution |
|---|---|---|
| [The AI Scientist](./papers/10_auto_research.md) | Nature 2026 | End-to-end autonomous AI research pipeline for ideation, experimentation, paper writing, and automated review |
| [TianJi](./papers/10_auto_research.md) | arXiv 2026 | WRF-centered multi-agent system for autonomous atmospheric mechanism verification |
| [Zephyrus](./papers/10_auto_research.md) | ICLR 2026 | Code-generating weather agent and benchmark for high-dimensional meteorological reasoning |
| [The AI Scientist-v2](./papers/10_auto_research.md) | arXiv 2025 | Template-free automated scientific discovery with agentic tree search and VLM-based review |
| [Robin](./papers/10_auto_research.md) | Nature 2026 | Lab-in-the-loop multi-agent system for hypothesis generation and biological discovery |
| [AutoMF](./papers/10_auto_research.md) | ICPR 2022 | AutoML / NAS framework for spatio-temporal meteorological forecasting architecture search |

</details>

---

## 📬 Contact

Questions or suggestions? Feel free to reach out via [Issues](https://github.com/zhengkai15/Awesome-Weather-Forecast/issues) or visit [zhengkai15.github.io](https://zhengkai15.github.io/) ლ(╹◡╹ლ)
