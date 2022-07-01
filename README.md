# Biochemical coordinate layout
Norwegian University of Science and Technology, 
Trondheim 2022\
Department of Biotechnology and Food Science\
[Machado lab](https://www.ntnu.edu/ibt/research/computational-biology/#/view/about) 


Thesis supervisor: [Daniel Machado](https://github.com/cdanielmachado/)\
Co-Supervisor: [Elisa Marquez](https://github.com/emarquezz/)

|Supplementary #|Name/Description|
|:-:|:-:|
|1|[Data collection](https://github.com/meidelien/Biochemical_coordinate_layout/tree/main/Data%20collection)|
|2|[Molecular descriptor calculation](https://github.com/meidelien/Biochemical_coordinate_layout/tree/main/Molecular%20descriptor%20calculation)|
|3|[Case study datasets](https://github.com/meidelien/Biochemical_coordinate_layout/tree/main/Case%20study%20datasets)|
|4|[Layout visualization](https://github.com/meidelien/Biochemical_coordinate_layout/tree/main/Case%20study%20datasets)|




## Dependencies
[![Powered by RDKit](https://img.shields.io/badge/Powered%20by-RDKit-3838ff.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQBAMAAADt3eJSAAAABGdBTUEAALGPC/xhBQAAACBjSFJNAAB6JgAAgIQAAPoAAACA6AAAdTAAAOpgAAA6mAAAF3CculE8AAAAFVBMVEXc3NwUFP8UPP9kZP+MjP+0tP////9ZXZotAAAAAXRSTlMAQObYZgAAAAFiS0dEBmFmuH0AAAAHdElNRQfmAwsPGi+MyC9RAAAAQElEQVQI12NgQABGQUEBMENISUkRLKBsbGwEEhIyBgJFsICLC0iIUdnExcUZwnANQWfApKCK4doRBsKtQFgKAQC5Ww1JEHSEkAAAACV0RVh0ZGF0ZTpjcmVhdGUAMjAyMi0wMy0xMVQxNToyNjo0NyswMDowMDzr2J4AAAAldEVYdGRhdGU6bW9kaWZ5ADIwMjItMDMtMTFUMTU6MjY6NDcrMDA6MDBNtmAiAAAAAElFTkSuQmCC)](https://www.rdkit.org/)

- Tested with Python 3.7, 3.8, 3.9, 3.10
- [RDKit](https://www.rdkit.org/docs/Install.html) 2021.03.5
  - To ensure compatibility with RDkit and required packages, build a new conda environment:
    - ``` $ conda create -c conda-forge -n YOUR_ENV_NAME_HERE rdkit```




1. Unpack chem_prop.zip & chem_xref.zip in the data folder [Source](https://www.metanetx.org/mnxdoc/mnxref.html)
   1. The unpacked files (chem_prop.tsv & chem_xref.tsv) have been added to 
   .gitignore because they are too large for git w/o git LFS 
2. Ignore emoticons in notebooks


### How-to (🚧 Under construction 🚧)

1. Create "Calc.csv" from your GEM (SBML format)
2. Run "DescriptorCalc.ipynb" to calculate chemical descriptors via RDkit
3. Standardize & apply PCA & append results to your output file in "PCA.ipynb" # Change this to include rankings and rename file to DataProcessing.ipynb or smthin
   1. Optional: Analyze descriptors via DescriptorAnalysis.ipynb
4. Get links between metabolites using BiGG identifiers for metabolites using "ReFramed.ipynb"
5. Run"DataVisualisation.ipynb" and input your desired GEMs & Pathways






