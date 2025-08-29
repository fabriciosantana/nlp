### Criando ambiente python usando venv

* Crie o ambiente virtual:
```bash
python -m venv .venvMCDIA

source .venvMCDIA/bin/activate

pip install --upgrade pip
```

* Instale pacotes python:
```bash
pip install notebook ipykernel pandas \
            jupyter matplotlib lxml \
            beautifulsoup4 html5lib \
            openpyxl requests sqlalchemy \
            seaborn scipy statsmodels \
            patsy scikit-learn pyarrow numba \
            #pytables
```

* Adicione o kernel do ambiente ao Jupyter:
```bash
python -m ipykernel install --user --name=mcdia-env --display-name="Python (mcdia-env)"
```

* Inicie o Jupyter Notebook:
```bash
jupyter notebook
```

### Criando ambiente python usando conda

```bash
conda create -y -n base

conda activate base
```

* Instale pacotes python:
```bash
conda install notebook ipykernel pandas \
            jupyter matplotlib lxml \
            beautifulsoup4 html5lib \
            openpyxl requests sqlalchemy \
            seaborn scipy statsmodels \
            patsy scikit-learn pyarrow numba \
            #pytables
```

```bash
python -m ipykernel install --user --name=conda-base --display-name="Python (conda base)"
```
```bash
jupyter kernelspec list
```