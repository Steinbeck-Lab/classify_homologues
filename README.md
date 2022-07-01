# A Cheminformatics Algorithm to Classify Homologous Series

## Introduction
Homologous series describe groups of chemical compounds containing a common core structure and a chain of growing repeating units.

This algorithm classifies homologous series defined by a user-specified repeating unit amongst an input dataset of molecules.
 
 
 
 
## Installation

The code can be installed directly from GitHub with:

```shell
$ pip install git+https://github.com/adelenelai/classify_homologues.git
```

The code can be installed in editable mode with:

```shell
$ git clone https://github.com/adelenelai/classify_homologues
$ cd src/classify_homologues
$ pip install -e .
```

## Usage

Then
```python classify_homologues.py <SMILES list> <Labels list> <repeating unit> 2>log```

Currently the only repeating unit is 'C', representing repeating alkyl groups i.e. -CH2-.

Try:

```
python classify_homols.py input/test1_smiles_23.csv input/test1_labels_23.csv C 2>log
```

Successful classification will generate an output directory containing .png plots of molecules, 1 plot per 1 classified series, and a .csv file containing machine-readable information on the classified series. 


Further optional outputs may be created depending on what the algorithm detects (e.g. molecules with no repeating units detected). Please see the sample output directories in this repository e.g., `output_test1/` for the example given above.



## License

This project is licensed under the Apache 2.0 License - see the [LICENSE](https://github.com/adelenelai/classify_homologues/blob/main/LICENSE) file for details.




## Authors

- [Adelene Lai](https://github.com/adelenelai)




## Acknowledgements
- 
## References

