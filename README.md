# Javascript-RandomForest

A browser-based Random Forest implementation in JavaScript.  
This project provides an interactive, no-dependency Random Forest library and demo web app for classification tasks—designed for education, technical exploration, or lightweight prototyping.

---

## Table of Contents

- [About](#about)
- [Features](#features)
- [Getting Started](#getting-started)
- [Basic Example](#basic-example)
- [Options](#options)
- [Usage Notes](#usage-notes)
- [License](#license)

---

## About

Javascript-RandomForest implements a configurable Random Forest classifier that runs entirely in your web browser.  
It lets you set forest and tree hyperparameters, load or generate datasets, and visualize classification performance.  
All model operations are performed locally with zero server-side dependencies.

---

## Features

- Forest configuration:
  - Set number of trees, maximum depth, minimum samples per split
  - Choose splitting criterion (`gini`, `entropy`)
  - Configure bootstrap sampling, max features, and more
- Training options:
  - Upload or paste CSV dataset
  - Synthetic multi-class data generation
  - Train/validation/test set splitting
- Monitoring:
  - Show accuracy, per-class metrics, out-of-bag (OOB) error (if bootstrap enabled)
  - Visualize per-tree predictions and overall forest voting
  - Display feature importances after fitting
- Model persistence:
  - Save/load trained forest models as JSON
- Inference:
  - Manual input for single sample prediction
  - Review individual and aggregate predictions

---

## Getting Started

### Requirements

- A modern web browser (Chrome, Firefox, Edge, Safari, etc.)

### Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/matthewJamesAbbott/Javascript-RandomForest.git
    ```
2. Open `index.html` in your browser.

_No server installation is required._

---

## Basic Example

To run a demo with synthetic data:

1. Open `index.html`
2. Adjust forest parameters (e.g., Trees: `10`, Max Depth: `5`, Bootstrap: `Enabled`)
3. Generate synthetic dataset (e.g., 3 classes, 100 samples/class)
4. Click **Train Forest**
5. View the model statistics and output predictions

To use your own data, upload a CSV or paste tabular data, then train and evaluate as above.

---

## Options

- **Number of Trees:** Control ensemble size
- **Max Depth:** Set limits on individual tree growth
- **Min Samples/Split:** Change minimum sample count per split
- **Splitting Criterion:** Choose between Gini or Entropy for classification splits
- **Max Features:** Limit number of features evaluated per split (`all`, `sqrt`, `log2`)
- **Bootstrap Samples:** Toggle bootstrapped sampling per tree
- **OOB Score:** Optionally report out-of-bag accuracy estimate when using bootstrap

---

## Usage Notes

- For best browser performance, recommended forest sizes are 5–50 trees with depths of 3–8 for medium-sized datasets.
- All computation and data handling are performed client-side—your data remains on your device.
- The provided synthetic data generator is best for demonstration, not for benchmarking.

---

## License

MIT License.  
You are free to use, modify, and distribute this project for any purpose.

---

## Demo Link

https://javascript-randomforest.vercel.app/
