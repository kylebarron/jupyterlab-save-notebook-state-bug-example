# jupyterlab-save-notebook-state-bug-example
Repro for bug saving binary buffers in jupyterlab

```sh
pixi install
pixi run python -m ipykernel install --user --name "$(basename "$PWD")"
pixi run jupyter lab
```

```sh
pixi run python -m nbconvert example.ipynb --to ipynb --stdout --execute > example_nbconvert.ipynb
```
