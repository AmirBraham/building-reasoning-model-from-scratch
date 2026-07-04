# Building a Reasoning Model From Scratch

Personal study repository following the book **"Build a Reasoning Model (From Scratch)"** by Sebastian Raschka.

## Structure

```
chapter_2/
  main.ipynb        # Load Qwen3-0.6B, tokenizer, and generate text
qwen3.py            # Local copy of the Qwen3 architecture for study/recoding
```

## Setup

Requires Python 3.10+ and [uv](https://docs.astral.sh/uv/) or plain pip.

### With pip + venv

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r https://raw.githubusercontent.com/rasbt/reasoning-from-scratch/refs/heads/main/requirements.txt
pip install jupyterlab ipykernel
python -m ipykernel install --user --name reasoning-from-scratch --display-name "Reasoning From Scratch"
```

### Launch JupyterLab

```bash
source .venv/bin/activate
jupyter lab
```

Open `chapter_2/main.ipynb` and select the **"Reasoning From Scratch"** kernel.

> The first run downloads the pretrained weights (~1.4 GB) from HuggingFace automatically.

## Reference

- Book repo: [rasbt/reasoning-from-scratch](https://github.com/rasbt/reasoning-from-scratch)
- Pretrained weights: [rasbt/qwen3-from-scratch](https://huggingface.co/rasbt/qwen3-from-scratch)
