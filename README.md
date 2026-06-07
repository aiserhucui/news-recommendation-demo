# Advanced AI for Climate Strategy, Industrial Decarbonization, & Generative LCA

An open-source research and development repository leveraging cutting-edge machine learning architectures—including Multi-Modal Foundation Models, Heterogeneous Graph Transformers (HGTs), Self-Supervised Earth Masked Autoencoders (EarthMAE), and Constrained Optimizers—to solve complex topology modeling, predictive, and capital allocation challenges in industrial sustainability and climate economics.

---

## 🔬 Core Research Pillars

This repository is organized into four primary pillars, each addressing a critical data, architectural, or economic bottleneck in global industrial decarbonization and product lifecycle pipelines.

### 1. Multi-Modal Foundation Models for Generative Life Cycle Assessment (CarbonAI-LCA)
* **File Link:** [`AI_LCA_fixed.ipynb`](./AI_LCA_fixed.ipynb)
* **Deployment & Rendering:** [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/aiserhucui/Sustainability-AI-Project/blob/main/AI_LCA_fixed.ipynb) [![Render nbviewer](https://img.shields.io/badge/render-nbviewer-orange.svg)](https://nbviewer.org/github/aiserhucui/Sustainability-AI-Project/blob/main/AI_LCA_fixed.ipynb)
* **Domain & Standards:** Sustainable AI · Industrial Ecology · ISO 14040/14044 · GHG Protocol · EU CSRD (Digital Product Passport)
* **Objective:** To automate, predict, and generate highly granular Product Carbon Footprints (PCFs) and complete Life Cycle Assessments at scale, bypassing traditional consulting bottlenecks ($10K–$100K costs and multi-month turnarounds).
* **Methodology:** Implements **CarbonAI v2.0**, an end-to-end multi-modal foundation model framework trained on real-world public LCA registries (OpenEPD Building Transparency, EPA GHG Emission Factors Hub, DEFRA UK Conversion Factors, and USDA LCA Commons). The architecture fuses unstructured Bill-of-Materials (BOM), manufacturing process topologies, and regional grid data. It structurally integrates **differentiable physics constraints** to preserve mass/energy balances, **proximal causal learning** to uncover structural emission drivers, **conditional diffusion** for generative material synthesis, and **constrained multi-objective Reinforcement Learning (RL)** for design-space exploration.
* **Key Capabilities:**
  * **Physics-Preserving Latent Space:** Enforces physical laws (thermodynamics and material conservation) via custom differentiable loss penalties during backpropagation, avoiding hallucinatory carbon accounting.
  * **Generative Alternative Synthesis:** Utilizes conditional diffusion to generate optimized product formulations and manufacturing adjustments that satisfy strict carbon reduction targets without compromising engineering specifications.
  * **Causal Attribution:** Moves beyond simple correlations to isolate true causal vectors of environmental impact across complex multi-step industrial processes.

### 2. Multi-Tier Scope 3 Emissions Modeling via Heterogeneous Graph Transformers
* **File Link:** [`GHG_Scope3_MultiTier_HGT.ipynb`](./GHG_Scope3_MultiTier_HGT.ipynb)
* **Deployment & Rendering:** [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/aiserhucui/Sustainability-AI-Project/blob/main/GHG_Scope3_MultiTier_HGT.ipynb) [![Render nbviewer](https://img.shields.io/badge/render-nbviewer-orange.svg)](https://nbviewer.org/github/aiserhucui/Sustainability-AI-Project/blob/main/GHG_Scope3_MultiTier_HGT.ipynb)
* **Objective:** To accurately model non-homogeneous entity metadata and deep physical topologies inherent in global, multi-tiered supply chains under severe data-scarcity conditions.
* **Methodology:** Implements a **Heterogeneous Graph Transformer (HGT)** architecture to capture the complex, multi-layered dependencies between upstream suppliers, refining facilities, logistics nodes, and end-products. Defined formally by the graph schema $\mathcal{G}=(\mathcal{V}, \mathcal{E}, \mathcal{T}_v, \mathcal{T}_e)$, the model leverages structural attention to propagate carbon intensity metrics across deep, unmapped supply networks.
* **Key Achievements:**
  * **Topology Resilience:** Successfully mapped deep upstream supply chain layers, robustly handling sparse primary data and highly skewed entity distributions.
  * **Baseline Outperformance:** Achieved a significant reduction in Mean Absolute Percentage Error (MAPE) for unmapped Tier-3+ supplier emissions compared to traditional, homogeneous Graph Convolutional Networks (GCNs).
  * **Attention Interpretability:** Extracted learned edge-attention weights to isolate and identify high-variance carbon chokepoints across the simulated industrial network.

### 3. Geospatial Self-Supervised Learning using Earth Masked Autoencoders (EarthMAE)
* **File Link:** [`EarthMAE_Self_Supervised_Final.ipynb`](./EarthMAE_Self_Supervised_Final.ipynb)
* **Deployment & Rendering:** [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/aiserhucui/Sustainability-AI-Project/blob/main/EarthMAE_Self_Supervised_Final.ipynb) [![Render nbviewer](https://img.shields.io/badge/render-nbviewer-orange.svg)](https://nbviewer.org/github/aiserhucui/Sustainability-AI-Project/blob/main/EarthMAE_Self_Supervised_Final.ipynb)
* **Objective:** To extract robust, high-fidelity representations from unlabelled remote sensing and geospatial data for scalable environmental monitoring and physical risk mitigation.
* **Methodology:** Leverages a **Self-Supervised Vision Transformer (ViT)** backbone with a masked autoencoder pre-training strategy. The model learns fundamental spatial-temporal patterns by reconstructing high-percentage masked imagery, creating highly transferable embeddings for downstream tasks like biomass estimation, land-use classification, and asset-level physical climate risk assessment.
* **Key Achievements:**
  * **High-Ratio Reconstruction:** Demonstrated robust spatial reconstruction capabilities even when operating at a heavy 75% pixel masking ratio, proving deep contextual understanding of regional land-cover features.
  * **Data Efficiency:** Downstream fine-tuning on highly limited labeled datasets achieved target convergence with substantially fewer labeled samples compared to a Vision Transformer trained completely from scratch.
  * **Transferability:** Embeddings demonstrated exceptional zero-shot stability across distinct geographic biomes, minimizing domain-shift errors when transferring from training regions to unmapped test zones.

### 4. Dynamic Marginal Abatement Cost Curve (MACC) Optimization
* **File Link:** [`Dynamic_MACC.ipynb`](./Dynamic_MACC.ipynb)
* **Deployment & Rendering:** [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/aiserhucui/Sustainability-AI-Project/blob/main/Dynamic_MACC.ipynb) [![Render nbviewer](https://img.shields.io/badge/render-nbviewer-orange.svg)](https://nbviewer.org/github/aiserhucui/Sustainability-AI-Project/blob/main/Dynamic_MACC.ipynb)
* **Objective:** To transform static, deterministic carbon abatement graphs into multi-period, path-optimized investment decision-support engines for multi-site operations.
* **Methodology:** Replaces traditional static MACC frameworks with a dynamic optimization engine. It models changing regulatory landscapes (e.g., carbon tax trajectories), capital expenditure depreciation, and technological learning curves over a rolling horizon, enabling industrial complexes to optimize their capital allocation paths under macroeconomic uncertainty.
* **Key Achievements:**
  * **Non-Convex Optimization Convergence:** Successfully formulated and solved a multi-period, constrained optimization problem, effectively avoiding local minima to isolate global path-optimal capital allocation strategies.
  * **Capital Efficiency:** The dynamic pathway identified an optimized deployment schedule that reduces the Net Present Cost (NPC) of industrial decarbonization over an extended 20-year horizon compared to static, cost-ranked baselines.
  * **Sensitivity Scaling:** Built-in multi-variable sensitivity analysis allows real-time shifts in carbon tax trajectories and technology learning rates, updating the optimal investment sequence computationally in seconds.

---

## 🛠️ Tech Stack & Theoretical Toolkit

* **Generative AI & Deep Learning:** PyTorch, Vision Transformers (ViT), Conditional Diffusion Models, Multi-Objective Reinforcement Learning (RL)
* **Graph Deep Learning:** PyTorch Geometric (PyG), Heterogeneous Graph Transformer (HGT) architectures, Attention Mechanisms
* **Mathematical Optimization & Causal Inference:** SciPy Optimization, NumPy, Pandas, Proximal Causal Learning Frameworks, Non-convex and Constrained Optimization
* **Interactivity & UI Rendering:** Voila, Jupyter Widgets (`ipywidgets`) for dynamic, real-time optimization visualization

---

## 📂 Repository Structure

```text
├── AI_LCA_fixed.ipynb                   # Multi-modal foundation model for generative LCA/PCF
├── GHG_Scope3_MultiTier_HGT.ipynb       # Supply chain graph transformer architecture
├── EarthMAE_Self_Supervised_Final.ipynb # Geospatial self-supervised vision model
├── Dynamic_MACC.ipynb                  # Multi-period carbon abatement optimization
├── requirements.txt                    # Project dependencies
└── README.md                           # Research Overview & Architectural Documentation
