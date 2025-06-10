## Accessing the Prostate158 Data Set

The training dataset (139 MRIs) is freely available at [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6481141.svg)](https://doi.org/10.5281/zenodo.6481141).

The test dataset consists of 19 additional MRIs and can be found at [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6592345.svg)](https://doi.org/10.5281/zenodo.6592345)

`pip install -U "monai[all]" pyyaml munch pandas opencv-python`

### Train an Anatomy Segmentation Model
Adapt the `data_dir`, the `train_csv`, `valid_csv` and `test_csv` file paths in the `anatomy.yaml`.
Then execute:  
```bash
python train.py --config anatomy.yaml

```