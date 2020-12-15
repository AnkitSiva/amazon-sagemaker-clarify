![Python package](https://github.com/aws/amazon-sagemaker-clarify/workflows/Python%20package/badge.svg)
![Python 3.6+](https://img.shields.io/badge/python-3.6+-blue.svg?style=flat)

# smclarify

Amazon Sagemaker Clarify

Bias detection and mitigation for datasets and models.

## Terminology

### Facet
A facet is column or feature that will be used to measure bias against. A facet can have value(s) that designates that sample as "***sensitive***".

### Label
The label is a column or feature which is the target for training a machine learning model. The label can have value(s) that designates that sample as having a "***positive***" outcome.

### Bias measure
A bias measure is a function that returns a bias metric.

### Bias metric
A bias metric is a numerical value indicating the level of bias detected as determined by a particular bias measure.

### Bias report
A collection of bias metrics for a given dataset or a combination of a dataset and model.

## Development
To set up your local development environment, run the following:

```
mkvirtualenv -p python3.7 YourVirtualEnvName
./devtool install_deps_dev
```

To run all tests:
```
./devtool all
```

Be sure to run tests and pre-commit hooks before submitting a PR.
