
## How to install the local python version during development
```bash
pip install -e .  # alternatively, use pip3
```

## How to install the extensions during development

### JupyterLab development

Via terminal, it's the same procedure as normal installation:

```bash
python -m pyforest install_labextension
```

It is also possible via Python:
```python
import pyforest
pyforest.install_labextension()  # takes 30-60s due to jupyter lab build
```

Run JupyterLab in watch mode
```
jupyter lab --watch
```

When you make changes on the javascript side, refresh the browser (clear cache) for changes to take effect.
### Jupyter Notebook

Via terminal, it's the same procedure as normal installation:

```bash
python -m pyforest install_nbextension
```

It is also possible via Python:
```python
import pyforest
pyforest.install_nbextension()
```

Run Notebook
```
jupyter notebook
```

When you make changes on the javascript side, you need to install nbextension again.
```bash
python -m pyforest install_nbextension
```

## Syntax formatting
We use `black` for formatting the Python code
