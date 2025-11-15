# dirichlet-mirt

To set up the Python environment:

```bash
CONDA_PLUGINS_AUTO_ACCEPT_TOS=yes conda create -n mirt python=3.10 -y
conda activate mirt
pip install -r requirements.txt
conda install -c conda-forge jupyterlab ipywidgets jupyterlab_widgets
```

To install latex-related packages (linux)

```bash
sudo apt update
sudo apt install -y texlive-latex-base texlive-latex-extra texlive-fonts-recommended texlive-fonts-extra cm-super dvipng fonts-liberation
```

## Download existing external evaluations

```bash
hf download ronanhansel/data-reeval-multi \
    --local-dir . \
    --repo-type dataset
```