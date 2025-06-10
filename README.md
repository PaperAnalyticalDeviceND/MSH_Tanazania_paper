# MSH Tanzania Paper

Analysis of MSH Tanzania PAD (Paper Analytical Device) drug testing data.

## Setup

1. Install `uv` if you haven't already
2. Create and activate virtual environment:
   ```bash
   uv venv .venv
   source .venv/bin/activate
   ```
3. Install dependencies:
   ```bash
   uv sync --all-extras
   ```

## Project Structure

- `data/` - Contains MSH Tanzania reads CSV files
   - MSHTanzaniaReads.csv - Results for each of the TFDA analysts evaluating 150 PADs each.  
- `notebooks/` - Jupyter notebooks for analysis
- `docs/` - Documentation files
  - `MHS‐Tanzania-NN-Results.md` - Neural network model results and performance metrics
- `.venv/` - Python virtual environment (not tracked in git)

## Running the Analysis

Start Jupyter and open the notebook:
```bash
jupyter notebook notebooks/MSHTanzaniaReads_mapping_test_dataset.ipynb
```

## Dataset Information

The neural network model results documented in `docs/MHS‐Tanzania-NN-Results.md` are based on the TFDA MSH-Tanzania dataset. The complete dataset used to train the neural network is available at:

**[TFDA MSH-Tanzania v2.0 Dataset](https://padproject.info/pad_dataset_registry/datasets/TFDA_MSH-Tanzania_v2.0/readme/)**

This dataset contains PAD (Paper Analytical Device) images for drug quality testing collected in Tanzania in collaboration with the Tanzania Food and Drug Authority (TFDA).
