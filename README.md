# P2P Process Mining and Exception Analysis

A process mining analysis of the BPI Challenge 2019 purchase-order event log,
focused on the procure-to-pay (P2P) process: 3-way match conformance,
process discovery, rework, and bottleneck analysis.

## Dataset

This project uses the **BPI Challenge 2019** event log (purchase order data
from a multinational coatings and paints company).

- **Official source:** [4TU.ResearchData - BPI Challenge 2019](https://data.4tu.nl/articles/dataset/BPI_Challenge_2019/12715853)
- **Alternative mirror:** [Kaggle - BPI Challenge 2019](https://www.kaggle.com/datasets/aaminaalzeri/bpi-challenge-2019)
  (convenience download; verify it matches the official source before use)
- **Format:** XES (~695MB uncompressed, ~1.6M events, ~252K cases)
- **Note:** The raw dataset file is not included in this repo (exceeds
  GitHub's file size limit). Download it from one of the links above and
  place it in the project folder before running the notebook.

## Setup

1. Download `BPI_Challenge_2019.xes` from the link above
2. Place it in this project's root folder
3. Install dependencies: `pip install pm4py graphviz`
4. Install Graphviz system binaries (see [graphviz.org/download](https://graphviz.org/download/))
5. Run `p2p_process_mining.ipynb`

## What this project covers

- Process discovery (directly-follows graph)
- Top process variants and happy-path %
- Case duration and bottleneck analysis
- Rework and 3-way match deviation detection
- Business write-up with findings
