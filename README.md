# AI for Climate Strategy & Industrial Decarbonization Frameworks

An open-source research repository leveraging advanced machine learning architectures—including Heterogeneous Graph Transformers (HGTs) and Self-Supervised Earth Masked Autoencoders (EarthMAE)—to solve complex optimization and topology modeling challenges in industrial sustainability and climate economics.

---

## 🔬 Core Research Frameworks & Key Achievements

This repository is organized into three primary pillars, addressing critical bottlenecks in climate data processing, supply chain visibility, and decarbonization economics.

### 1. Multi-Tier Scope 3 Emissions Modeling via Heterogeneous Graph Transformers
* **File:** `GHG_Scope3_MultiTier_HGT.ipynb`
* **Deployment & Rendering:**
    [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/aiserhucui/Sustainability-AI-Project/blob/main/GHG_Scope3_MultiTier_HGT.ipynb) &nbsp; [![View on NBViewer](https://img.shields.io/badge/render-nbviewer-orange.svg)](https://nbviewer.org/github/aiserhucui/Sustainability-AI-Project/blob/main/GHG_Scope3_MultiTier_HGT.ipynb)
* **Objective:** To model non-homogeneous entity metadata and complex physical topologies inherent in global supply chains.
* **Methodology:** Implements a **Heterogeneous Graph Transformer (HGT)** architecture to capture the intricate, multi-layered dependencies between suppliers, processing facilities, and end-products. By explicitly accounting for distinct node and edge types—defined formally by the graph schema $\mathcal{G} = (\mathcal{V}, \mathcal{E}, \mathcal{T}_v, \mathcal{T}_e)$—the model propagates carbon intensity metrics across deep supply networks to accurately estimate upstream Scope 3 footprints under severe data-scarcity conditions.
* **🏆 Key Achievements:**
    * **Topology Resilience:** Successfully mapped deep upstream supply chain layers, robustly handling sparse primary data and highly skewed entity distributions.
    * **Baseline Outperformance:** Achieved a significant reduction in Mean Absolute Percentage Error (MAPE) for unmapped Tier-3+ supplier emissions compared to traditional, homogeneous Graph Convolutional Networks (GCNs).
    * **Attention Interpretability:** Extracted learned edge-attention weights to isolate and identify the highest-variance carbon chokepoints across the simulated industrial network.

---

### 2. Geospatial Self-Supervised Learning using Earth Masked Autoencoders (EarthMAE)
* **File:** `EarthMAE_Self_Supervised_Final.ipynb`
* **Deployment & Rendering:**
    [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/aiserhucui/Sustainability-AI-Project/blob/main/EarthMAE_Self_Supervised_Final.ipynb) &nbsp; [![View on NBViewer](https://img.shields.io/badge/render-nbviewer-orange.svg)](https://nbviewer.org/github/aiserhucui/Sustainability-AI-Project/blob/main/EarthMAE_Self_Supervised_Final.ipynb)
* **Objective:** To extract robust, high-fidelity representations from unlabelled remote sensing and geospatial data for environmental monitoring.
* **Methodology:** Leverages a **Self-Supervised Vision Transformer (ViT)** backbone with a masked autoencoder pre-training strategy. The model learns fundamental spatial-temporal patterns by reconstructing high-percentage masked imagery, creating highly transferable embeddings for downstream tasks like biomass estimation, land-use classification, and physical climate risk assessment.
* **🏆 Key Achievements:**
    * **High-Ratio Reconstruction:** Demonstrated robust spatial reconstruction capabilities even when operating at a heavy 75% pixel masking ratio, proving deep contextual understanding of regional land-cover features.
    * **Data Efficiency:** Downstream fine-tuning on highly limited labeled datasets achieved target convergence with substantially fewer labeled samples compared to a Vision Transformer trained completely from scratch.
    * **Transferability:** Embeddings demonstrated exceptional zero-shot stability across distinct geographic biomes, minimizing domain-shift errors when transferring from training regions to unmapped test zones.

---

### 3. Dynamic Marginal Abatement Cost Curve (MACC) Optimization
* **File:** `Dynamic_MACC.ipynb`
* **Deployment & Rendering:**
    [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/aiserhucui/Sustainability-AI-Project/blob/main/Dynamic_MACC.ipynb) &nbsp; [![View on NBViewer](https://img.shields.io/badge/render-nbviewer-orange.svg)](https://nbviewer.org/github/aiserhucui/Sustainability-AI-Project/blob/main/Dynamic_MACC.ipynb)
* **Objective:** To transform static carbon abatement models into dynamic, multi-period investment decision-support tools.
* **Methodology:** Replaces traditional deterministic MACC frameworks with a dynamic optimization engine. It models changing regulatory landscapes, capital expenditure depreciation, and technological learning curves over extended horizons, enabling multi-site industrial operations to path-optimize their net-zero roadmaps under uncertainty.
* **🏆 Key Achievements:**
    * **Non-Convex Optimization Convergence:** Successfully formulated and solved a multi-period, constrained optimization problem, effectively avoiding local minima to isolate global path-optimal capital allocation strategies.
    * **Capital Efficiency:** The dynamic pathway identified an optimized deployment schedule that reduces the Net Present Cost (NPC) of industrial decarbonization over an extended 20-year horizon compared to static, cost-ranked baselines.
    * **Sensitivity Scaling:** Built-in multi-variable sensitivity analysis allows real-time shifts in carbon tax trajectories and technology learning rates, updating the optimal investment sequence computationally in seconds.

---

## 🛠️ Tech Stack & Theoretical Toolkit

* **Graph Deep Learning:** PyTorch Geometric (PyG), Heterogeneous Graph Attention Networks
* **Computer Vision / SSL:** PyTorch, Vision Transformers (ViT), Masked Autoencoding
* **Mathematical Optimization:** SciPy Optimization, NumPy, Pandas (Non-convex and constrained frameworks)
* **Interactivity & Deployment:** Voila, Jupyter Widgets (for interactive optimization visualization)

---

## 📂 Repository Structure

```text
├── GHG_Scope3_MultiTier_HGT.ipynb       # Supply chain graph transformer architecture
├── EarthMAE_Self_Supervised_Final.ipynb # Geospatial self-supervised vision model
├── Dynamic_MACC.ipynb                  # Multi-period carbon abatement optimization
├── requirements.txt                    # Project dependencies
└── README.md                           # Research Overview
