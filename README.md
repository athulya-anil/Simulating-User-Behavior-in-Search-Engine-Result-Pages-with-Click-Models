# Simulating User Behavior in Search Engine Result Pages with Click Models

## Overview
This project explores user behavior on Search Engine Result Pages (SERPs) using click models, including the Position-Based Model (PBM), Cascade Model, and an Enhanced PBM. By simulating and analyzing user clicks, the project aims to improve the understanding of position bias and contextual relevance in search ranking systems.

---

## Features
- Implementation of multiple click models:
  - **Position-Based Model (PBM)**: Accounts for position bias.
  - **Cascade Model**: Simulates sequential scanning behavior.
  - **Random Model**: Serves as a baseline for comparison.
  - **Enhanced PBM**: Integrates query-specific weights and contextual features.
- Evaluation using key metrics:
  - **Click-Through Rate (CTR)**
  - **Normalized Discounted Cumulative Gain (nDCG)**
  - **Mean Squared Error (MSE)**
- Visualization of click distributions across positions.
- Alignment with real-world click data trends.

---

## Dataset
- **Source**: Yandex Personalized Web Search Challenge dataset.
- **Description**:
  - Training sessions: 34,573,630
  - Test sessions: 797,867
  - Relevance grades:
    - 0: Irrelevant (Dwell time < 50).
    - 1: Relevant (Dwell time: 50–399).
    - 2: Highly Relevant (Dwell time ≥ 400).

---

## Installation

### Prerequisites
- Python 3.7 or above
- Libraries:
  - `numpy`
  - `pandas`
  - `matplotlib`
  - `scikit-learn`
  - `scipy`

### Steps
1. Clone the repository - git clone https://github.com/athulya-anil/Simulating-User-Behavior-in-Search-Engine-Result-Pages-with-Click-Models.git
2. Install requirements -
3. Run the collab notebook cells one by one

## Evaluation Metrics
- **Click-Through Rate (CTR):** Measures the average click probability by position.
- **nDCG:** Evaluates ranking quality compared to an ideal ranking.
- **MSE:** Quantifies errors between predicted and actual clicks.

---

## Observations
- **PBM:** Effectively captures position bias but overestimates clicks for lower ranks.
- **Cascade Model:** Aligns well for top positions but struggles for lower ones.
- **Enhanced PBM:** Outperforms other models, achieving superior nDCG (0.75) and CTR (35%).

---

## Results
- **PBM:**  
  - nDCG: 0.67  
  - CTR: Overestimates for lower ranks.
- **Cascade Model:**  
  - nDCG: 0.70  
  - Performs well for top positions.
- **Enhanced PBM:**  
  - nDCG: 0.75  
  - Closely aligns with real-world trends.

---

## Future Work
- Address variability in user behavior for lower-ranked results.
- Incorporate diverse query scenarios and user-specific preferences.

---

## License
This project is licensed under the [MIT License](LICENSE).

---

## Authors
- **Athulya Anil**  
  University of Massachusetts Amherst  
  [athulyaanil@umass.edu](mailto:athulyaanil@umass.edu)
  
- **Durga Nirmaleswaran**  
  University of Massachusetts Amherst  
  [dnirmaleswaran@umass.edu](mailto:dnirmaleswaran@umass.edu)

---

## Acknowledgments
- Yandex Personalized Web Search Challenge dataset.

### References
- Joachims et al. (2005)
- Chapelle & Zhang (2009)
- Craswell et al. (2008)

   
