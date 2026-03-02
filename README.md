# fedsa_public

This repository documents the data processing and analysis workflow used in Field Effect Detection by Spectral Analysis (FEDSA). Experimental signals acquired from nanoparticle suspensions are treated as dynamic light scattering–type data to validate the expected frequency-domain behavior and to support particle-size–related interpretations. For in vivo breast tissue measurements, the workflow computes power spectra and summarizes them into normalized frequency bands, which are then used for multivariate analysis and PCA-based logistic regression.

In addition to apparent model fitting, the repository includes leakage-safe internal validation using patient-grouped cross-validation (leave-one-patient-out and grouped 5-fold), where all measurements from the same participant are kept within the same fold to prevent within-subject leakage. Performance is reported from pooled out-of-fold participant-level predictions (ROC-AUC, sensitivity, and specificity), with uncertainty quantified via patient-level bootstrap confidence intervals.

The Jupyter Notebook [*data_processing.ipynb*](https://github.com/davidalejandromiranda/fedsa_public/blob/main/data_processing.ipynb) provides interactive visualization of the experimental data and reproduces the full pipeline, from signal conditioning and band extraction to modeling and internal validation. This repository accompanies the associated manuscript and is intended to support transparency and reproducibility of the proof-of-concept study.

## How to cite this work?

David A. Miranda, Janeth Fernandez-Pinto and Álvaro Gómez-Torrado (2026). davidalejandromiranda/fedsa_public: Frequency-Domain Dynamic Light Scattering (FEDSA) for In Vivo Screening of Breast Tissue Abnormalities: A Proof-of-Concept Study (v1.1). Zenodo. [https://doi.org/10.5281/zenodo.18832019](https://doi.org/10.5281/zenodo.18832019)

[old version] David Alejandro Miranda Mercado (2023). davidalejandromiranda/fedsa_public: Exploring the breast cancer risk detection by dynamic light scattering (v1.0). Zenodo. [https://doi.org/10.5281/zenodo.8200226](https://doi.org/10.5281/zenodo.8200226)

## DOI

[DOI: 10.5281/zenodo.18832019](https://doi.org/10.5281/zenodo.18832019)

[old version]

[![DOI](https://zenodo.org/badge/668259331.svg)](https://zenodo.org/badge/latestdoi/668259331)

## BibTeX

```
@software{Miranda2026,
  author       = {David A. Miranda, Janeth Fernandez-Pinto and Álvaro Gómez-Torrado},
  title        = {davidalejandromiranda/fedsa_public: Frequency-Domain Dynamic Light Scattering (FEDSA) for In Vivo Screening of Breast Tissue Abnormalities: A Proof-of-Concept Study},
  month        = march,
  year         = 2026,
  publisher    = {Zenodo},
  version      = {v1.1},
  doi          = {10.5281/zenodo.18832019},
  url          = {https://doi.org/10.5281/zenodo.18832019}
}
```

Old version:
```
@software{Miranda2023,
  author       = {David A. Miranda},
  title        = {davidalejandromiranda/fedsa_public: Exploring the breast cancer risk detection by dynamic light scattering},
  month        = jul,
  year         = 2023,
  publisher    = {Zenodo},
  version      = {v1.0},
  doi          = {},
  url          = {[https://doi.org/10.5281/zenodo.8200226](https://doi.org/10.5281/zenodo.8200226)}
}
```

## Licence

This work is under the MIT license.