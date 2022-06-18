# nilearn-extra

**Nilearn Extra** is a small drop-in extension for *[Nilearn](https://nilearn.github.io/) (Statistics for NeuroImaging in Python)*. Currently, it provides some additional functional connectivity measures.



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
- Transfer Entropy (`kind="transfer entropy"`) between regions X and Y is amount of uncertainty reduced in Y by knowing the past values of X. Note that transfer entropy is a asymmetric measure, so is the connectivity matrix.

# Optional dependencies

```bash
# for transfer entropy connectivity
pip install pyinform
```

## Contributing

We use GitHub to fork and manage pull requests.

## License

BSD 3-Clause License. See the [LICENSE](LICENSE) file.
