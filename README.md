Core Research Frameworks & Key Achievements
This repository is organized into three primary pillars, addressing critical bottlenecks in climate data processing, supply chain visibility, and decarbonization economics.

1. Multi-Tier Scope 3 Emissions Modeling via Heterogeneous Graph Transformers
File: GHG_Scope3_MultiTier_HGT.ipynb

Objective: To model non-homogeneous entity metadata and complex physical topologies inherent in global supply chains.

Methodology: Implements an HGT architecture to capture the intricate, multi-layered dependencies between suppliers, processing facilities, and end-products. By accounting for distinct node and edge types, the model propagates carbon intensity metrics across deep supply networks to accurately estimate upstream Scope 3 footprints under data-scarce conditions.

🏆 Key Achievements:

Topology Resilience: Successfully mapped up to [X] tiers of upstream supply chain depth, handling highly sparse primary data environments.

Baseline Outperformance: Achieved a [XX]% reduction in Mean Absolute Percentage Error (MAPE) for unmapped Tier-3+ supplier emissions compared to standard homogeneous Graph Convolutional Networks (GCNs).

Attention Interpretability: Extracted learned edge-attention weights to isolate and identify the top [X] highest-variance carbon chokepoints across the simulated industrial network.

2. Geospatial Self-Supervised Learning using Earth Masked Autoencoders (EarthMAE)
File: EarthMAE_Self_Supervised_Final.ipynb

Objective: To extract robust, high-fidelity representations from unlabelled remote sensing and geospatial data for environmental monitoring.

Methodology: Leverages a Self-Supervised Vision Transformer (ViT) backbone with a masked autoencoder pre-training strategy. The model learns fundamental spatial-temporal patterns by reconstructing high-percentage masked imagery, creating highly transferable embeddings for downstream tasks like biomass estimation, land-use classification, and physical climate risk assessment.

🏆 Key Achievements:

High-Ratio Reconstruction: Demonstrated robust spatial reconstruction capabilities even when operating at a [e.g., 75%] pixel masking ratio, proving deep contextual understanding of land cover features.

Data Efficiency: Downstream fine-tuning on limited labeled datasets achieved target convergence with [XX]% fewer labeled samples compared to a Vision Transformer trained completely from scratch.

Transferability: Embeddings demonstrated zero-shot stability across distinct geographic biomes, minimizing domain-shift errors when transferring from training regions to test regions.

3. Dynamic Marginal Abatement Cost Curve (MACC) Optimization
File: Dynamic_MACC.ipynb

Objective: To transform static carbon abatement models into dynamic, multi-period investment decision-support tools.

Methodology: Replaces traditional deterministic MACC frameworks with a dynamic optimization engine. It models changing regulatory landscapes, capital expenditure depreciation, and technological learning curves over extended horizons, enabling multi-site industrial operations to path-optimize their net-zero roadmaps under uncertainty.

🏆 Key Achievements:

Non-Convex Optimization Convergence: Successfully formulated and solved a multi-period, constrained optimization problem, avoiding local minima to find global path-optimal capital allocation strategies.

Capital Efficiency: The dynamic pathway identified an optimized deployment schedule that reduces the Net Present Cost (NPC) of industrial decarbonization by [XX]% over a [e.g., 20-year] horizon compared to a static, cost-ranked baseline.

Sensitivity Scaling: Built-in multi-variable sensitivity analysis allows real-time shifts in carbon tax trajectories and technology learning rates, updating the optimal investment sequence in under [X] seconds.
