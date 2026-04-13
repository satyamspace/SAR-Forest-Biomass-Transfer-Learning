# SAR-Forest-Biomass-Transfer-Learning

**Satyam Shah | MSc GIS, University of Leicester**

### Project: Transfer Learning Across Forest Types for Biomass Estimation


---
This notebook demonstrates a proof-of-concept pipeline for the proposed PhD project.
It uses **real OSM boundaries**, **Sentinel-1 SAR data** from GEE, **GEDI L4A biomass**, and 
**ETH Global Canopy Height** to characterise domain shift and baseline transfer learning between:
- 🇩🇪 **Bavarian Forest NP** — temperate mixed forest (source domain)
- 🇦🇺 **Daintree Rainforest** — tropical rainforest (target domain)
- 🇦🇺 **Lamington NP** — subtropical rainforest (target domain)

**Pipeline steps:**
1. Real OSM boundary loading & visualisation
2. Sentinel-1 SAR feature extraction (VV, VH, RVI, NDPI)
3. Annual composites & temporal trend analysis
4. Domain shift quantification (Euclidean distance, KS-test)
5. GEDI L4A biomass reference integration
6. ETH Canopy Height → allometric AGB
7. Naive baseline transfer (Random Forest)
8. Domain adaptation (feature alignment via MMD)
9. Uncertainty quantification (MC Dropout)
10. Results summary & next steps
