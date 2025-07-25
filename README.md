# CutoffChaos

This repository accompanies the manuscript “Chaotic behavior in geometric river channel evolution over multiple cutoff cycles.”

We use [meanderpy](https://github.com/zsylvester/meanderpy) to model meandering rivers. We run a reference channel and a set of initially perturbed channels forward to study the divergence in channel evolution due to cutoff events.

![Ensemble channel divergence GIF](https://github.com/braydennoh/CutoffChaos/blob/main/figure/1.gif)

Meanderpy is a Lagrangian model, so channel evolution is naturally represented as moving nodes. To systematically quantify divergence between channels, we project the centerlines onto a fixed Eulerian grid and calculate the separation using the Lyapunov exponent.

* **`figure1.ipynb`**: Runs ensembles of reference and perturbed channels and generates ensemble divergence visualizations, like  
  
  ![Ensemble divergence example](https://github.com/braydennoh/CutoffChaos/blob/main/figure/asesaega.png)


* **`figure2.ipynb`**: Computes the Lyapunov exponent with varying perturbation magnitude.  
  
  ![Lyapunov exponent example](https://github.com/braydennoh/CutoffChaos/blob/main/figure/paperfigure2.png)


* **`figure3.ipynb`**: Computes the Lyapunov exponent with varying grid size.  
  
  ![Lyapunov exponent example](https://github.com/braydennoh/CutoffChaos/blob/main/figure/paperfigure3.png)



## How to Use

1. **Clone this repository:**

   ```
   git clone https://github.com/braydennoh/CutoffChaos.git
   cd CutoffChaos
   ```

2. **Install dependencies** (`meanderpy`, `numpy`, `matplotlib`):

   ```
   pip install -r requirements.txt
   ```

3. **Run Notebooks**
   Open `figure1.ipynb`, `figure2.ipynb`, and `figure3.ipynb` in Jupyter or Colab and run cells sequentially.

   * `figure1.ipynb` generates diverging channel ensembles.
   * `figure2.ipynb` calculates and plots the Lyapunov exponent with varying perturbation magnitude.  
   * `figure3.ipynb` calculates and plots the Lyapunov exponent with varying grid size.  


## Reference

If you use this code, please cite our paper:
**Noh & Wani, 2025. "Chaotic behavior in geometric river channel evolution over multiple cutoff cycles."**
