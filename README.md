The goal of this repository is to apply statistical methods and machine learning techniques to real-world scientific data to uncover patterns and validate experimental models.

## LHC (Large Hadron Collider) Analysis
### Data Source 
* Open data from CERN (ATLAS/CMS detectors).

### Focus
* Processing particle collision event records to identify signal vs. background noise.

### Methodology
* **Signal vs. Background:** Classified simulated LHC events (Higgs signal vs. QCD background jets).
* **Jet Substructure:** Utilized physical variables like **Jet Mass** and the **Energy Correlation Function ratio ($d_2$)** to distinguish two-pronged Higgs decays from "noisy" QCD jets.
* **Significance Optimization:** Quantified the Significance improvement using the discovery significance formula:  
    $$\Sigma = \frac{N_{\text{signal}}}{\sqrt{N_{\text{background}}}}$$
* **Grid Search:** Iteratively tested $d_2$ cut values to identify the threshold that yields the maximum statistical significance.

### Key Results
* **Optimal Cut:** Identified $d_2 \le 0.517$ as the optimal selection threshold.
* **Discovery Potential:** Successfully reached a significance level of **$3\sigma$** on the training dataset.
* **Validation:** Applied the optimized selection criteria to a separate high-$p_T$ (1000-1200 GeV/c) dataset to confirm the robustness of the discovery.
