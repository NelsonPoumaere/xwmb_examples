# xWMB workshop (OSM2026, Glasgow, 25/02/26)

## Clone this repository

This repo contains the different notebooks and associated files for use during the workshop.
Go to the location of your choice on your computer and run the following command line to download the repo:

```
git clone git@github.com:NelsonPoumaere/xwmb_examples.git
```
Or you can download the zip file directly from this page.

## Install xWMB

**Minimal installation within an existing environment**
```bash
conda install -c conda-forge xwmb=0.6.0
```

**Simple pip install**
```bash
pip install xwmb==0.6.0
```

**Installing from scratch using `conda`**

This is the recommended mode of installation for developers.
```bash
git clone git@github.com:hdrake/xwmb.git
cd xwmb
conda env create -f docs/environment.yml
conda activate docs_env_xwmb
pip install -e .
```

You can verify that the package was properly installed by confirming it passes all of the tests with:
```bash
pytest -v
```

**Launching a Jupyter session**

If you used the devs install option, you can launch a Jupyterlab instance using this environment with:
```bash
python -m ipykernel install --user --name docs_env_xwmb --display-name "docs_env_xwmb"
jupyter-lab
```

You can also launch a Jupyter Notebook session with `jupyter notebook`, and choose the `docs_env_xwmb` kernel.

If you used the pip or conda install option, then you should have xwmb and its dependencies available with the default `Python 3` kernel.

## Download the datasets

Several datasets can be downloaded for the workshop.
The notebooks already include download queries, but in order to save some time, you can already download the datasets directly from the Zenodo archives.

### MOM6_global tutorial

Download the `MOM6_global_example_sigma2_budgets_v0_0_6.nc` file in [https://zenodo.org/records/15420739] and place it in the data/ directory.

### CROCO tutorial

Download the four `*rrexnum*` files in [https://zenodo.org/records/18469910] and place them in the data/ directory.

### SOSE tutorial

Download first the `march` netcdf file in [https://zenodo.org/records/18681726] and place it in the data/ directory.
Optionally, you can also download the `january` dataset.
