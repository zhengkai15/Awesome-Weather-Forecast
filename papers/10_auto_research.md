# 🤖 AI Auto-Research

LLM-agent systems and adjacent AI-driven discovery workflows for automating parts of the scientific research lifecycle: idea generation, literature review, experiments, paper writing, peer review, rebuttal, dissemination, and autonomous scientific experimentation.

---

- **[A Vision for Auto Research with LLM Agents]** (arXiv 2025) — *Conceptual multi-agent framework for modularizing the full scientific workflow.*
  - 📄 [Paper](https://doi.org/10.48550/arXiv.2504.18765) | 💻 [Code](https://github.com/worldbench/awesome-auto-research)
  - 👥 Chengwei Liu et al. (Nanyang Technological University / Nankai University)
  - 🧠 Model / framework: LLM-based multi-agent system covering **Literature → Idea → Method → Experiment → Paper → Evaluation → Rebuttal → Promotion**.
  - 🧪 Experiment: preliminary explorations across selected stages; mainly demonstrates feasibility rather than a fully benchmarked end-to-end system.
  - ⚠️ Limitations: vision-oriented paper; lacks rigorous quantitative evaluation, strong end-to-end experiments, and clear evidence that agents can reliably judge novelty or scientific correctness.
  - ✅ Conclusion: Auto-research should be treated as a modular, interpretable, and optimizable research process; LLM agents may reduce workflow fragmentation, but human validation remains necessary.

- **[The AI Scientist / Towards End-to-End Automation of AI Research]** (Nature 2026) — *End-to-end autonomous AI research pipeline that can generate complete machine-learning papers.*
  - 📄 [Paper](https://doi.org/10.1038/s41586-026-10265-5) | 💻 [Code](https://github.com/SakanaAI/AI-Scientist)
  - 👥 Chris Lu et al. (Sakana AI / Oxford / UBC / Vector Institute)
  - 🧠 Model / framework: foundation-model-based agentic system for **ideation, novelty checking, experiment coding, tree-search experimentation, plotting, manuscript writing, and automated peer review**.
  - 🔧 Models / tools: uses modern foundation models inside an agentic pipeline; template-free version uses models such as OpenAI o3 for reasoning/idea critique, Claude Sonnet 4 for coding, GPT-4o for vision-language tasks, and o4-mini for review-style reasoning.
  - 🧪 Experiment: evaluated in template-based and template-free settings; generated ML research papers; submitted 3 AI-generated papers to an ICLR workshop with organizers' consent; 1 paper reached likely-accept workshop quality but was withdrawn by protocol.
  - ⚠️ Limitations: only 1/3 workshop submissions passed; workshop acceptance bar is lower than main conferences; failures include shallow ideas, incorrect implementations, weak methodology, duplicated figures, hallucinated or inaccurate citations, and risks of flooding peer review.
  - ✅ Conclusion: demonstrates that full AI-generated research artifacts can sometimes pass a real peer-review process, but current systems are not yet reliable enough for consistent high-quality, top-tier scientific research.


---

- **[TianJi: An Autonomous AI Meteorologist for Discovering Physical Mechanisms in Atmospheric Science]** (arXiv 2026) — *WRF-centered multi-agent system for autonomous atmospheric mechanism verification.*
  - 📄 [Paper](https://doi.org/10.48550/arXiv.2603.27738) | 💻 [Code](https://github.com/zwww-www/output)
  - 👥 Kaikai Zhang et al. (Nanjing University of Information Science and Technology / China University of Petroleum)
  - 🧠 Model / framework: LLM-driven multi-agent “AI meteorologist” with two modules: academic-seminar-style hypothesis generation and WRF-centered hypothesis verification.
  - 🔧 Tools / models: researcher, host, and chief-scientist agents for debate-based hypothesis refinement; master / worker agents for WPS-WRF configuration, FNL data handling, simulation execution, NetCDF tensor analysis, and visualization.
  - 🧪 Experiment: validated on squall-line cold-pool dynamics and Typhoon In-fa track-deflection mechanisms; also tested simple WRF analysis and plotting tasks.
  - ⚠️ Limitations: experiments are mainly short-term mesoscale cases; broader climate-scale, coupled Earth-system, data-assimilation, and multi-model generalization remain untested.
  - ✅ Conclusion: shows that LLM agents can move from black-box weather prediction toward autonomous physical-mechanism testing, but still needs wider validation and stricter benchmarking against expert workflows.

- **[Zephyrus: An Agentic Framework for Weather Science]** (ICLR 2026) — *Code-generating weather agent and benchmark for reasoning over high-dimensional meteorological data.*
  - 📄 [Paper](https://doi.org/10.48550/arXiv.2510.04017) | 💻 [Code](https://github.com/Rose-STL-Lab/Zephyrus)
  - 👥 Sumanth Varambally et al. (UC San Diego)
  - 🧠 Model / framework: ZephyrusWorld + Zephyrus agents; LLMs write and execute Python code to query weather data, run forecasts, simulate climate, compute climatology, and refine answers through observations.
  - 🔧 Tools / models: WeatherBench 2 / ERA5 interface, geolocator, Stormer weather forecaster, JCM climate simulator, climatology module, FastAPI execution server; includes Direct and Reflective agent variants.
  - 🧪 Experiment: builds ZephyrusBench with 2230 QA samples across 49 tasks, covering lookups, forecasts, anomaly detection, extreme events, report generation, and counterfactual reasoning.
  - ⚠️ Limitations: hard tasks remain difficult; report generation and long-range global climate discussion are weak; reflective execution improves some models but not consistently across all LLMs.
  - ✅ Conclusion: tool-grounded weather agents substantially outperform text-only LLMs and make meteorological data more interactive, but current systems still cannot reliably perform expert-level scientific reasoning on complex weather phenomena.

- **[The AI Scientist-v2: Workshop-Level Automated Scientific Discovery via Agentic Tree Search]** (arXiv 2025) — *Template-free AI research system with tree-search experimentation and VLM-based review.*
  - 📄 [Paper](https://doi.org/10.48550/arXiv.2504.08066) | 💻 [Code](https://github.com/SakanaAI/AI-Scientist-v2)
  - 👥 Yutaro Yamada, Robert Tjarko Lange, Cong Lu et al. (Sakana AI / UBC / Oxford / Vector Institute)
  - 🧠 Model / framework: generalized idea generation, experiment-manager agent, progressive agentic tree search, parallel experiment execution, VLM figure critique, manuscript writing, and AI reviewing.
  - 🔧 Improvement over v1: removes dependence on human-written code templates and replaces linear experimentation with stage-wise tree search: preliminary investigation, hyperparameter tuning, research agenda execution, and ablation studies.
  - 🧪 Experiment: generated three fully autonomous ICLR workshop submissions; one received workshop-level accept scores before being withdrawn according to the pre-arranged evaluation protocol.
  - ⚠️ Limitations: quality is still below top-tier main-conference standards; failure modes include citation hallucination, shallow methodology, figure-caption errors, limited experiments, and possible dataset leakage.
  - ✅ Conclusion: demonstrates that AI-generated research can sometimes reach peer-reviewable workshop quality, but robust scientific rigor and reliable verification remain unresolved.

- **[A Multi-Agent System for Automating Scientific Discovery]** (Nature 2026) — *Robin system for AI-driven hypothesis generation and lab-in-the-loop biological discovery.*
  - 📄 [Paper](https://doi.org/10.1038/s41586-026-10652-y) | 💻 [Code](https://github.com/Future-House/robin)
  - 👥 Ali E. Ghareeb et al. (FutureHouse / Oxford / Fordham University)
  - 🧠 Model / framework: Robin coordinates literature-search agents Crow and Falcon with data-analysis agent Finch to generate hypotheses, select assays, analyze experimental data, and refine therapeutic candidates.
  - 🔧 Tools / models: PaperQA2-based literature agents, LLM-judged candidate ranking, multi-trajectory Finch analysis in Jupyter notebooks, flow-cytometry and RNA-seq analysis pipelines.
  - 🧪 Experiment: targeted dry age-related macular degeneration; proposed RPE phagocytosis enhancement, identified Y-27632 and ripasudil, analyzed flow cytometry and RNA-seq, and highlighted ABCA1 as a possible mechanistic target.
  - ⚠️ Limitations: laboratory execution remains human-operated; the case study is one disease area; biological interpretation and clinical translation require further experimental validation.
  - ✅ Conclusion: provides strong evidence for lab-in-the-loop AI discovery, where agents can connect literature synthesis, experiment selection, data analysis, and iterative hypothesis refinement.

- **[Accelerating Earth Science Discovery via Multi-Agent LLM Systems]** (Frontiers in AI 2025) — *Perspective and prototype architecture for multi-agent geoscience data discovery.*
  - 📄 [Paper](https://doi.org/10.3389/frai.2025.1674927) | 💻 [Code](https://github.com/CliDyn/pangaeaGPT)
  - 👥 Dmitrii Pantiukhin et al. (Alfred Wegener Institute)
  - 🧠 Model / framework: perspective article centered on PANGAEA GPT, a LangChain / LangGraph multi-agent pipeline for heterogeneous geoscientific data repositories.
  - 🔧 Tools / architecture: centralized supervisor agent dynamically delegates to domain agents for oceanography, geology, climatology, ecology, retrieval, data conversion, analysis, visualization, validation, and reporting.
  - 🧪 Experiment / evidence: presents PANGAEA GPT as a proof-of-concept for natural-language access, RAG-grounded search, and tool-mediated geoscientific workflows rather than a controlled benchmark.
  - ⚠️ Limitations: lacks rigorous quantitative evaluation against traditional workflows; metadata quality, tool misuse, hallucination, validation, privacy, and compute cost remain key issues.
  - ✅ Conclusion: multi-agent LLM systems could make Earth-science archives more searchable and reusable, especially for underused heterogeneous datasets, but robust validation layers are essential.

- **[AutoMF: Spatio-Temporal Architecture Search for the Meteorological Forecasting Task]** (ICPR 2022) — *AutoML / NAS approach for data-driven meteorological forecasting.*
  - 📄 [Paper](https://doi.org/10.1109/ICPR56361.2022.9956271) | 💻 Code: not released / not specified in the provided paper
  - 👥 Xinbang Zhang, Qizhao Jin, Shiming Xiang, Chunhong Pan (Chinese Academy of Sciences / University of Chinese Academy of Sciences)
  - 🧠 Model / framework: AutoMF, a multi-level neural architecture search framework for meteorological forecasting, combining a multi-modal fusion network and a spatio-temporal MF-LSTM network.
  - 🔧 Method: differentiable sampling-based architecture search with progressive search; explicitly adds terrain information and solar elevation angle to model spatial heterogeneity and temporal periodicity.
  - 🧪 Experiment: evaluated on ERA5 data over China and Southeast Asia for temperature, humidity, U/V wind, and precipitation forecasts at 6–36 h lead times; outperformed LR, ConvLSTM, PredRNN, PredRNN++, TrajGRU, and MIM in RMSE.
  - ⚠️ Limitations: regional dataset and relatively short lead times; purely data-driven architecture search does not provide physical mechanism interpretation; global-scale and more-variable forecasting are left for future work.
  - ✅ Conclusion: automated architecture search can improve meteorological deep-learning models by adapting network structure to multi-modal and spatio-temporal weather dynamics.

- **[Autonomous Agents for Scientific Discovery: Orchestrating Scientists, Language, Code, and Physics]** (arXiv 2026) — *Broad survey and conceptual framework for LLM-based scientific agents.*
  - 📄 [Paper](https://doi.org/10.48550/arXiv.2510.09901) | 💻 Code: not released / survey paper
  - 👥 Lianhao Zhou et al. (Texas A&M / Harvard / MIT / UCLA / UIUC and collaborators)
  - 🧠 Model / framework: survey taxonomy rather than a single system; frames scientific agents as orchestrators of human scientists, natural language, computer code, and physical information.
  - 🔧 Taxonomy: organizes autonomous discovery into **Hypothesis Discovery → Experimental Design & Execution → Result Analysis & Refinement**, with emphasis on tool use, tool creation, memory, planning, and verification.
  - 🧪 Evidence base: synthesizes LLM-agent systems across biology, medicine, chemistry, materials, physics, geoscience, and other domains; proposes an information-theoretic view using entropy, verifiability, and dissipation.
  - ⚠️ Limitations: conceptual and survey-oriented; does not benchmark a new system; many reviewed agents remain brittle, domain-specific, hard to validate, and dependent on human oversight.
  - ✅ Conclusion: scientific agents are becoming a general interface between ideas, code, tools, and empirical evidence, but the hardest open problem is still reliable verification of novel claims.

---

## Overall Takeaway

Auto-research is moving from local assistance toward multi-stage research agents. The current frontier can generate plausible research artifacts quickly, including ideas, tasks, literature summaries, code, plots, papers, reviews, limitations, benchmark questions, and dissemination materials. In domain sciences, the same pattern now appears in weather, geoscience, materials, and biology as agents are connected to numerical models, data archives, robotic labs, and specialized analysis pipelines.

However, the central bottleneck is no longer generation itself, but **verification**: whether ideas are genuinely novel, code implements the intended method, experiments are meaningful, citations are faithful, automated reviews are fair, outputs are physically or biologically valid, and conclusions are reproducible.

The most reliable near-term pattern is therefore:

> AI handles retrieval, drafting, coding, plotting, review support, limitation generation, workflow orchestration, data querying, repeated experiment execution, and preliminary result interpretation; humans retain control over novelty judgment, experimental design, scientific interpretation, verification, authorship, and accountability.
