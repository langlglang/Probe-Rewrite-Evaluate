# Probe-Rewrite-Evaluate

Code and data for the paper *Probe-Rewrite-Evaluate*.

## Contents

| Path | Description |
|------|-------------|
| `Probe_writing_experiment_code.ipynb` | Probe training and iterative prompt-rewriting experiments |
| `ResponseAndClassification.ipynb` | Model response generation and classification |
| `layer_23.pt` | Trained linear probe weights (layer 23) |
| `data/dataset.yaml` | Prompt dataset |
| `data/prompts_and_scores.csv` | Prompts with probe scores |
| `final_output.csv`, `optimized.csv`, `iterative_rewrite_results.csv`, `results_with_scores.csv` | Experiment outputs |
| `violin_probe_scores_*.png` | Probe score distribution figures |

## Setup

```bash
pip install -r requirements.txt
```

Set the API keys used by the notebooks as environment variables:

```bash
export HF_TOKEN=...            # Hugging Face (gated Llama models)
export OPENAI_API_KEY=...
export ANTHROPIC_API_KEY=...
export GOOGLE_API_KEY=...      # also read as GEMINI_API_KEY in ResponseAndClassification.ipynb
```
