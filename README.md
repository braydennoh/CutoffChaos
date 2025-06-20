# CutoffChaos

This repository accompanies the manuscript “Chaotic behavior in geometric river channel evolution over multiple cutoff cycles.”

We use [meanderpy](https://github.com/zsylvester/meanderpy) to model meandering rivers. We run a reference channel and a set of initially perturbed channels forward to study the divergence in channel evolution due to cutoff events.

<p align="center">
  <img src="https://github.com/braydennoh/CutoffChaos/blob/main/figure/1.gif" alt="Ensemble channel divergence GIF" width="400"/>
</p>

**Key idea:**
Meanderpy is a Lagrangian model, so channel evolution is naturally represented as moving nodes. To systematically quantify divergence between channels, we project the centerlines onto a fixed Eulerian grid and calculate the separation using the Lyapunov exponent.

* **`figure1.ipynb`**: Runs ensembles of reference and perturbed channels and generates ensemble divergence visualizations, like
  ![Ensemble divergence example](https://github.com/braydennoh/CutoffChaos/blob/main/figure/2.png)

* **`figure2.ipynb`**: Computes the Lyapunov exponent by measuring divergence in the Eulerian map over time.

---

## How to Use

1. **Clone this repository:**

   ```
   git clone https://github.com/braydennoh/CutoffChaos.git
   cd CutoffChaos
   ```

2. **Install dependencies** (requires `meanderpy`, `numpy`, `matplotlib`, etc.):

   ```
   pip install -r requirements.txt
   ```

3. **Run Notebooks**
   Open `figure1.ipynb` and `figure2.ipynb` in Jupyter or Colab and run cells sequentially.

   * `figure1.ipynb` generates diverging channel ensembles.
   * `figure2.ipynb` calculates and plots the Lyapunov exponent.

---

## Reference

If you use this code, please cite our paper:
**Noh & Wani, 2025. "Chaotic behavior in geometric river channel evolution over multiple cutoff cycles."**

---
