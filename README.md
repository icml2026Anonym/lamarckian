# lamarckian

Anonymous code and notebooks for reproducing the experiments in the accompanying ICML submission.

# Anonymous ICML Submission: Reproducibility Package

This repository contains the implementation and Google Colab notebooks used to produce the experimental results reported in the accompanying ICML submission.

## Repository Structure
The core experimental artifacts are compressed in `lamarckian.zip`. This archive contains:
- **Colab Notebooks (`.ipynb`)**: Separate notebooks for each dataset (Higgs, Hepmass, GloVe, SIFT) and sequence length configuration.
- **Verifiable Results**: All notebooks are saved with **cell outputs preserved**. Reviewers can open these notebooks to immediately verify the execution logs, timings, and resulting metrics without needing to re-run the code.

## Verification & Reproducibility

### Option 1: Quick Verification (Recommended)
1. Download and unzip `lamarckian.zip`.
2. Open any `.ipynb` file in a local viewer, Jupyter, or Google Colab.
3. Scroll through the cells to inspect the pre-computed logs, runtime metrics, and final outputs that match the tables in the paper.

### Option 2: Full Reproduction
To re-run the experiments from scratch:
1. Upload the specific notebook to Google Colab.
2. Acquire the standard public datasets (Higgs, Hepmass, GloVe, SIFT) and upload them to your environment (e.g., Google Drive).
   - *Note: Due to size and licensing, datasets are not included in this repo.*
3. Update the file paths in the first cell to point to your data location.
4. Run all cells. All randomized components use fixed seeds (documented in the notebooks) to ensure repeatability.

## Notes
- **Hardware**: The reported results (and preserved outputs) were generated on Google Colab Pro instances. Runtimes may vary on different hardware.
- **Dependencies**: Notebooks include cells to install necessary dependencies at runtime.
