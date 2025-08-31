# STATS 201: Replication of Multi-Scale Energy Grid Benchmarks

This repository contains code to replicate parts of the benchmark experiments from the paper:
**"A multi-scale time-series dataset with benchmark for machine learning in decarbonized energy grids"** by Ospina et al.

*   **Paper:** [https://www.nature.com/articles/s41597-022-01657-z](https://www.nature.com/articles/s41597-022-01657-z)
*   **Original Repository:** (https://github.com/tamu-engineering-research/Open-source-power-dataset)
## System Configuration & Setup

The dataset is large and hosted on Zenodo. The code in the notebook will handle downloading it.

### Option 1: Cloud Environment (Highly Recommended - Google Colab with High-RAM Runtime)
1.  **Open the Notebook in Colab:**
    [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/STATS201/stats201-multiscale-energy-grids/blob/main/code/system_config_experiments.ipynb)
    *(This badge will work after you upload the notebook to your repo.)*

2.  **Runtime Type:** Go to `Runtime` -> `Change runtime type` and select **High-RAM** under `Hardware accelerator`. This is crucial for loading the larger files in the dataset.

3.  **Run the Notebook:** Execute the cells. The notebook will download the data from Zenodo and install necessary packages.

### Option 2: Local Setup
1.  **Clone the repository:**
    ```bash
    git clone https://github.com/STATS201/stats201-multiscale-energy-grids.git
    cd stats201-multiscale-energy-grids
    ```

2.  **Create and activate a Conda environment:**
    ```bash
    conda create -n stats201-multiscale python=3.9 # Matches paper's version
    conda activate stats201-multiscale
    ```

3.  **Install required packages:**
    The notebook uses standard data science libraries. You can install them with:
    ```bash
    pip install numpy pandas matplotlib scikit-learn requests
    ```

4.  **Run the Jupyter Notebook:**
    ```bash
    jupyter notebook
    ```
    Navigate to the `code/` folder and open `system_config_experiments.ipynb`.
    **Warning:** The full dataset is over 5 GB. Ensure you have sufficient disk space and RAM.
