# Large Language Model-assisted Text Mining (LATeM) 

This repository contains the code used in the research paper "Analyzing the transition of elastin research from 1975 to 2024 through large language model-assisted text mining (LATeM)."

## Overview

The code implements the Large Language Model-assisted Text Mining (LATeM) approach, which combines traditional text mining techniques with advanced Large Language Models to analyze research trends in scientific literature. This implementation specifically focuses on processing and analyzing bibliographic data.

## Features

- Automated processing of bibliographic data from Excel/CSV files
- Analysis of research trends across different time periods (1990-1999, 2000-2009, 2010-2019, 2020-2024)
- Identification of new terms and growing research topics
- Export functionality for analysis results

## Requirements

- Python 3.10 or higher
- pandas
- Google Colab environment (for the notebook version)

Required Python packages:
```
pandas
io
re
os
```

## Usage

1. Upload your Excel or CSV file containing bibliographic data
2. The script will process the following periods:
   - 1990-1999
   - 2000-2009
   - 2010-2019
   - 2020-2024

3. Choose your preferred output format (CSV or Excel)
4. The script will generate:
   - New terms analysis for each period
   - Growth terms analysis showing increasing usage rates

## Input File Format

Your input file should contain columns with the following naming pattern:
- `word (YYYY-YYYY)`: Contains terms/keywords
- `count (YYYY-YYYY)`: Contains frequency counts

Example column names:
- `word (1990-1999)`
- `count (1990-1999)`
- `word (2000-2009)`
- `count (2000-2009)`
etc.

## Output Files

The script generates two types of output files for each time period:
1. `new_terms_{period}.csv/xlsx`: Lists terms that first appeared in that period
2. `growth_terms_{period}.csv/xlsx`: Lists terms with significant growth in usage

## Citation

If you use this code in your research, please cite our paper:

```bibtex
@article{LATeM2024,
  title={Uncovering new psychoactive substances research trends using large language model-assisted text mining (LATeM)},
  year={2024}
  // Additional citation details will be added upon publication
}
```

## License

[MIT License](LICENSE)

## Contact

For questions about the code or research, please open an issue in this repository.

## Related Resources

- [Link to the full research paper]()
- [Additional supplementary materials]()
