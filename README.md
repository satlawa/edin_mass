# edin_mass

Version 0.1<br>

Predict the volume of timber of planned thinnings. This project uses the Crown Height Model (CHM) (remote sensing) and follows the following steps.
for every forest stand:

1. clip CHM raster with forest stand boundries
2. calculate 10 | 20 | 30 | ... | 80 | 90 percentile of tree heights
3. append to rest of data

Finally we use machine learing algorithms RF, SVM to create a model.

## Install

### Install enviroment
Although it is not strictly necessary to create an environment with conda, it is highly recommended to use conda to assure no problems with already installed package versions. If you have conda (Anaconda or Miniconda) already installed please skip point 1. and continue with 2. If you are unsure if you have conda installed you can use the following command to check:<br>
```which conda```

1. Download and install conda from:<br>
  * Anaconda (recommended): https://www.anaconda.com/products/individual<br>
or from:<br>
  * Miniconda :             https://repo.anaconda.com/miniconda/<br>

2. Create an environment<br>
```conda create --name geo```

3. Activate the newly created environment<br>
```conda activate geo```

4. Install packages<br>
```conda install python=3.8.5 numpy=1.21.2 pandas=1.3.4 matplotlib=3.4.3 reportlab=3.5.67 ipykernel```

5. Add kernel to Jupiter Notebook<br>
```python -m ipykernel install --user --name pdf_reports```

6. Deactivate kernel<br>
```conda deactivate```

## Copy repository

1. Navigate to home directory<br>
```cd ~```

2. Make a new directory and navigate to it<br>
```mkdir -p Code/python & cd Code/python```

3. Clone the GitHub environment (or download the zipped version)<br>
```git clone https://github.com/satlawa/obf_obf_autrep_bzhs.git```

## Prepare Data
Download all necessary data from SAP and put the files in the appropriate folder.<br>
