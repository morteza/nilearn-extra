# Nilearn Extra

**Nilearn Extra** is a small add-on for *[Nilearn](https://nilearn.github.io/) (Statistics for NeuroImaging in Python)*. It currently adds some functional connectivity measures to the mix.

## Installation

```bash
pip install nilearn-extra
```

## Usage

```diff
- from nilearn.connectome import ConnectivityMeasure
+ from nilearn_extra.connectome import ConnectivityMeasure
```

## Extra Connectivity Matrices

Nilearn Extra supports two additional connectivity matrices:
- Chatterjee XiCorr (`kind="chatterjee"`) is a new correlation coefficient as described in [Chatterjee (2019)](https://arxiv.org/abs/1909.10140).
- Transfer Entropy (`kind="transfer entropy"`) between regions X and Y is amount of uncertainty reduced in Y by knowing the past values of X. Transfer entropy is an asymmetric measure, so is the connectivity matrix.

# Optional Dependencies

```bash
# transfer entropy connectivity requires `pyinform` package.
pip install pyinform
```

## Contributing

We use GitHub to fork and manage pull requests.

## Acknowledgements
This project is supported by the Luxembourg National Research Fund (ATTRACT/2016/ID/11242114/DIGILEARN).



## License

BSD 3-Clause License. See the [LICENSE](LICENSE) file.
