# Contributing to Awesome-Weather-Forecast

Thank you for your interest in contributing! This list collects high-quality papers on AI-driven weather forecasting. We welcome community submissions.

---

## 📋 How to Submit a Paper

1. **Fork** this repository
2. Create a branch: `git checkout -b add/paper-name`
3. Add the paper entry to the appropriate file under `papers/`
4. Submit a **Pull Request** with the title format: `[Add] ModelName (Venue Year)`

> For bug fixes or corrections, use `[Fix] description` as the PR title.

---

## 📝 Paper Entry Format

Each entry follows this format:

```markdown
- **[ModelName]** (Venue Year) — *One-sentence description of the core contribution.*
  - 📄 [Paper](https://arxiv.org/abs/xxxx.xxxxx) | 💻 [Code](https://github.com/org/repo) *(omit Code line if not available)*
  - 👥 First Author et al.
```

**Example:**

```markdown
- **[Pangu-Weather]** (Nature 2023) — *3D Earth-specific transformer for accurate medium-range global weather forecasting.*
  - 📄 [Paper](https://www.nature.com/articles/s41586-023-06185-3) | 💻 [Code](https://github.com/198808xc/Pangu-Weather)
  - 👥 Kaifeng Bi et al.
```

---

## 📂 Which File to Edit?

| Category | File |
|---|---|
| Medium-Range Forecast (1–15 days) | `papers/01_medium_range.md` |
| NowCasting (0–6 hours) | `papers/02_nowcasting.md` |
| Super Resolution / Downscaling | `papers/03_super_resolution.md` |
| Data Assimilation | `papers/04_data_assimilation.md` |
| Extreme Weather (incl. Typhoon) | `papers/05_extreme_weather.md` |
| Seasonal & Climate | `papers/06_seasonal_climate.md` |
| Data Compression | `papers/07_compression.md` |
| Foundation Models | `papers/08_foundation_models.md` |
| Recent Highlights (2025–2026) | `papers/09_2025_2026_new.md` |

---

## ✅ Inclusion Criteria

- The paper must be **published or posted on arXiv** (peer-reviewed venues preferred)
- The paper must be **directly relevant** to AI/ML-driven weather/climate forecasting
- Please provide a **working link** to the paper
- Avoid duplicates — check existing entries before submitting

## ❌ What We Don't Include

- Papers unrelated to meteorology/atmospheric science
- Entries without verifiable paper links
- Duplicate entries already in the list

---

## 🙏 Thank You

Every contribution, big or small, helps make this list better for the entire AI4Science community!
