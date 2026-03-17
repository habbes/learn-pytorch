# Learn [PyTorch](https://pytorch.org/)

- [Deep Learning with PyTorch: A 60 Minute Blitz](https://docs.pytorch.org/tutorials/beginner/deep_learning_60min_blitz.html)
- [PyTorch Beginner YouTube Series](https://www.youtube.com/playlist?list=PL_lsbAsL_o2CTlGHgMxNrKhzP97BaG9ZN)
- [Learn the basics](https://docs.pytorch.org/tutorials/beginner/basics/intro.html)
- [What is `torch.nn` really](https://docs.pytorch.org/tutorials/beginner/nn_tutorial.html)

# Setup

- This repo uses [`uv`](https://docs.astral.sh/uv) to manage python an dependencies
  - We also use `uv` to [install `PyTorch`](https://docs.astral.sh/uv/guides/integration/pytorch) instead of the official [PyTorch installation guide](https://pytorch.org/get-started/locally).
  - TODO: make sure CUDA support is added on Windows and Linux

Install and use [`uv`](https://docs.astral.sh/uv/) to manage the python project, environments and run
scripts within the context of the environment.

This repo is [`uv` project](https://docs.astral.sh/uv/guides/projects) and runs runs scripts
and install dependencies in its isolated python environment.

To update the environment manually, of if you don't see the `.venv` folder in the project root, run

```bash
uv sync
```

You can run the Jupyter notebooks (`.ipynb`) in VS Code using the [Jupyter extension](https://marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter)

Make VS Code Jupyter extension is using the project's environment to execute code. If it prompts to you
choose an environment, select custom path and enter `.venv/bin/python` (macOS, Linux) or `.venv/Scripts/python.exe` (Windows).

The python environment in use is displayed at the top right corner of the notebook.

![Python env disabled in VS Code notebook](vscode-notebook-python-env.png)
