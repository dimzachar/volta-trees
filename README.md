# VoltaTrees 🍃
![CI](https://github.com/siboehm/lleaves/workflows/CI/badge.svg)
[![Documentation Status](https://readthedocs.org/projects/lleaves/badge/?version=latest)](https://lleaves.readthedocs.io/en/latest/?badge=latest)
[![Downloads](https://pepy.tech/badge/lleaves)](https://pepy.tech/project/lleaves)

A LLVM-based compiler for LightGBM and XGBoost decision trees.

`VolaTree` converts trained LightGBM and XGBoost models to optimized machine code, speeding-up prediction by ≥10x.

## Example

```python
import voltatrees as vt

model = vt.XGBoostRegressor.Model(model_file="NYC_taxi/model.txt")
model.compile()
model.predict(df)
```

## Installation

(Need to add it to pip)

## Benchmarks

(TBD on bare-metal machine)

## Development 

```bash
conda env create
conda activate voltatrees
git clone git clone https://github.com/VoltaML/volta-trees.git
cd volta-trees/
pip install -e .
```
