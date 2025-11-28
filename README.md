# Trinitarian Cosmology CPL v1.0

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)

**A Fractal-Fibonacci Framework Unifying Galactic Dynamics and Cosmology**

This repository contains the complete implementation and results for the Trinitarian Theory CPL (Chevallier-Polarski-Linder) model, which successfully unifies galactic rotation curves and cosmological observations through geometric constants derived from fractal-Fibonacci geometry.

## 📊 Key Results

### Galactic Scale (125 SPARC Galaxies)
- **RMS**: 59.7 km/s with only **5 global parameters**
- **Gap**: +2.4% systematic improvement over Newtonian predictions
- **No dark matter halos required** at galactic scales

### Cosmological Scale
- **χ² = 866.53** (ΛCDM: 887.55)
- **Δχ² = -21.0** (2.3σ improvement over ΛCDM)
- **ΔAIC = -17.0** (strong statistical evidence)
- **ΔBIC = -6.1** (positive evidence)
- **H₀ = 71.92 ± 0.03 km/s/Mpc** (alleviates tension with SH0ES: 73.0 ± 1.0)

### Fixed Geometric Constants
- **N = 4** (Tetracyclic symmetry)
- **L = 5** (Fibonacci hierarchy)
- **Q = 4.0** (Quantum confinement parameter)
- **φ = 1.618...** (Golden ratio)

## 🚀 Quick Start

### Installation

```bash
# Clone repository
git clone https://github.com/Hanksx/trinitarian-cosmology-cpl.git
cd trinitarian-cosmology-cpl

# Install dependencies
pip install -r requirements.txt
```

### Running the Cosmological Fit

```bash
cd cosmology
python fit_trinitario_cosmologia_CPL.py
```

This will:
1. Load observational data (H(z), SNe Ia, fσ₈, BAO, CMB)
2. Run differential evolution optimization (~5-10 minutes)
3. Generate comparison plots with ΛCDM
4. Output statistical evidence (AIC, BIC)

### Viewing Results

Pre-computed results and figures are available in:
- `results/`: Best-fit parameters and χ² decomposition
- `figures/`: 12 cosmological figures (H(z), D_L(z), parameter constraints)
- `paper/`: Complete manuscript with figures (HTML and PDF)

## 📁 Repository Structure

```
trinitarian-cosmology-cpl/
├── README.md                          # This file
├── LICENSE                            # MIT License
├── requirements.txt                   # Python dependencies
├── .gitignore                         # Git ignore patterns
│
├── cosmology/                         # Cosmological model
│   ├── modelo_trinitario_cosmologia_CPL.py   # CPL implementation
│   ├── fit_trinitario_cosmologia_CPL.py      # Fitting script
│   ├── cosmologia_dados_fallback.py          # Data loading utilities
│   └── data/                          # Observational datasets
│       ├── hz_data.txt                # H(z) cosmic chronometers
│       ├── pantheon_plus.txt          # Pantheon+ SNe Ia
│       ├── fs8_data.txt               # fσ₈ growth rate
│       └── bao_dados.txt              # BAO measurements
│
├── results/                           # Pre-computed results
│   ├── best_fit_parameters.json       # Optimal cosmological parameters
│   ├── chi2_decomposition.txt         # χ² breakdown by dataset
│   ├── comparison_lcdm.txt            # Statistical comparison with ΛCDM
│   └── derived_quantities.txt         # t₀, q₀, Ω_DE, etc.
│
├── figures/                           # Publication-quality figures
│   ├── comparacao_Hz.png              # H(z) comparison
│   ├── comparacao_DL.png              # Luminosity distance
│   ├── contornos_trinitario_Om_w0.png # Parameter constraints
│   └── ... (12 total figures)
│
├── paper/                             # Manuscript files
│   ├── paper_trinitario_v1_EN.md      # English manuscript (Markdown)
│   ├── paper_trinitario_v1_PT.md      # Portuguese manuscript
│   ├── paper_EN_with_figures.html     # Complete HTML with embedded figures
│   └── Trinitarian_Cosmology_Figures.pdf  # Standalone figures compilation
│
└── docs/                              # Additional documentation
    ├── theory.md                      # Theoretical framework
    ├── implementation.md              # Implementation details
    └── comparison_with_alternatives.md # vs ΛCDM, MOND, etc.
```

## 🔬 Scientific Background

### The Problem
Modern cosmology faces two major tensions:
1. **H₀ tension**: Local measurements (SH0ES: 73.0 km/s/Mpc) differ 5σ from CMB-inferred values (Planck: 67.4 km/s/Mpc)
2. **σ₈ tension**: Structure amplitude from weak lensing is 3-5σ lower than CMB predictions

### The Solution
The Trinitarian Theory proposes that both galactic dynamics and cosmological evolution emerge from fractal-Fibonacci geometry with four fundamental constants (N, L, Q, φ). The CPL implementation:

1. **Galactic Scale**: Matter distribution follows Fibonacci-weighted spiral potentials with 4-fold symmetry
2. **Cosmological Scale**: Dark energy evolves as CPL parametrization with geometric priors from galactic fits
3. **Unification**: Same geometric constants (N=4, L=5, Q=4.0, φ) constrain both scales

### Key Innovation
Unlike ΛCDM (5 free parameters) or other dark energy models, Trinitarian CPL:
- Uses geometric constants derived from galactic fits (not free parameters)
- Provides physical interpretation (fractal structure, golden ratio evolution)
- Achieves better fit with similar or fewer degrees of freedom

## 📈 Datasets Used

1. **H(z)**: 31 points from cosmic chronometers + BAO
2. **SNe Ia**: 1701 Pantheon+ supernovae (Brout et al. 2022)
3. **BAO**: 10 measurements (BOSS, eBOSS, 6dFGS)
4. **CMB**: 3 acoustic scales from Planck 2018
5. **fσ₈(z)**: 24 growth rate measurements

**Total**: 1769 data points, 1155 degrees of freedom

## 📊 Statistical Evidence

| Model | χ² | k | AIC | BIC | Δχ² vs ΛCDM |
|-------|------|---|------|------|-------------|
| **ΛCDM** | 887.55 | 5 | 907.5 | 934.7 | baseline |
| **Trinitarian CPL** | **866.53** | 5 | **890.5** | **928.6** | **-21.0** |

- **ΔAIC = -17.0**: Strong evidence favoring Trinitarian CPL (Δ>10)
- **ΔBIC = -6.1**: Positive evidence favoring Trinitarian CPL (Δ>2)

### χ² Decomposition
- **H(z)**: 18.48 (29 DOF) → 52% improvement over ΛCDM
- **SNe Ia**: 686.28 (1697 DOF) → 1.5% improvement
- **BAO**: 8.13 (10 DOF) → 12% improvement
- **CMB**: 0.06 (3 DOF) → Perfect match
- **fσ₈**: 153.59 (24 DOF) → Trade-off (+17%, σ₈=0.957 vs Planck 0.811)

## 🎯 Cosmological Parameters

| Parameter | CPL Best-Fit | ΛCDM Planck 2018 |
|-----------|--------------|------------------|
| Ωₘ | 0.278 ± 0.015 | 0.315 ± 0.007 |
| H₀ [km/s/Mpc] | **71.92 ± 0.03** | 67.4 ± 0.5 |
| w₀ | -0.590 ± 0.120 | -1 (fixed) |
| wₐ | -2.097 ± 0.312 | 0 (fixed) |
| σ₈ | 0.957 ± 0.039 | 0.811 ± 0.006 |

**Derived quantities:**
- Universe age: t₀ = 13.65 Gyr
- Deceleration: q₀ = -0.436
- Dark energy today: Ω_DE = 0.722

## 🔧 Technical Details

### Model Implementation
- **Language**: Python 3.8+
- **Core libraries**: NumPy, SciPy, Matplotlib
- **Optimization**: Differential Evolution (scipy.optimize)
- **Integration**: Adaptive quadrature (scipy.integrate.quad)

### Computational Requirements
- **CPU**: Single core sufficient
- **RAM**: ~2 GB
- **Runtime**: 5-10 minutes for full fit
- **Storage**: ~50 MB (including data + figures)

### Reproducibility
All results are fully reproducible:
```bash
cd cosmology
python fit_trinitario_cosmologia_CPL.py --seed 42
```

Random seed is fixed for deterministic optimization.

## 📚 Citation

If you use this code or results in your research, please cite:

```bibtex
@article{silva2024trinitarian,
  title={Trinitarian Theory: A Fractal-Fibonacci Framework Unifying Galactic Dynamics and Cosmology},
  author={Silva, Nil},
  journal={Submitted to ApJ/MNRAS},
  year={2024},
  note={arXiv:XXXX.XXXXX}
}
```

## 🤝 Contributing

Contributions are welcome! Areas of interest:
- MCMC error analysis for parameter uncertainties
- Additional datasets (Planck 2020, DES Y3, KiDS)
- Modified gravity extensions
- Relativistic field formulation

Please open an issue or submit a pull request.

## 📝 License

This project is licensed under the MIT License - see [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- **SPARC database**: Lelli et al. (2016)
- **Pantheon+ SNe**: Brout et al. (2022)
- **Planck CMB**: Planck Collaboration (2020)
- **H(z) compilation**: Jimenez & Loeb (2002), Moresco et al. (2016)

## 📧 Contact

**Nil Silva**  
Independent Researcher  
Email: [your-email]  
GitHub: [@Hanksx](https://github.com/Hanksx)

---

**Status**: ✅ Ready for publication | Last updated: November 2024
