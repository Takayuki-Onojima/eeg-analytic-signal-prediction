# Direct Prediction of the Complex-Valued Analytic Signal of EEG from Raw Multichannel Data

Supplementary material and code for:

> Takayuki Onojima and Takashi Imai,
> "Direct Prediction of the Complex-Valued Analytic Signal of EEG from Raw Multichannel Data,"
> *IEEE Journal of Biomedical and Health Informatics*. <!-- TODO: add volume, pages, year, DOI -->

## Overview

This study predicts the complex-valued analytic signal (real and imaginary components) of EEG at posterior
electrodes (PO7, PO3, POz, PO4, PO8) directly from causal, raw 63-channel EEG input (1-s window, 500 samples).
The proposed model (TCN-NLL) uses a dilated causal temporal convolutional network with a Gaussian
negative log-likelihood objective. A training strategy with masked signal inputs (MSI) improves robustness
when electrodes are missing.

## Repository structure

```
.
├── supplementary/
│   └── Supplementary_Material.pdf   # Supplementary Material (Sections S1–S8)
└── src/                             # Source code (coming soon)
```

## Supplementary Material

[`supplementary/Supplementary_Material.pdf`](supplementary/Supplementary_Material.pdf) contains:

| Section | Content |
|---|---|
| S1 | Implementation details of the baseline models (TCN-NLL, CNN-NLL, LSTM-NLL) |
| S2 | Leakage-free target construction and data splitting |
| S3 | Circular phase-error metric |
| S4 | Controlled comparison of the MSI probability |
| S5 | AR order-selection analysis (AIC/BIC) |
| S6 | Repeated-split cross-subject robustness analysis |
| S7 | Supplementary statistical comparisons |
| S8 | Effect of the MSI probability on normalized residual distributions |

## Code

**Coming soon.** The source code will be released in the [`src/`](src/) directory.

## Citation

<!-- TODO: replace with the final BibTeX entry once published. -->

```bibtex
@article{onojima_analytic_signal_eeg,
  author  = {Onojima, Takayuki and Imai, Takashi},
  title   = {Direct Prediction of the Complex-Valued Analytic Signal of {EEG} from Raw Multichannel Data},
  journal = {IEEE Journal of Biomedical and Health Informatics},
  year    = {TODO},
  doi     = {TODO}
}
```
