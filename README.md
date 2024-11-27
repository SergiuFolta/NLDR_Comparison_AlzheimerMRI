# NLDR Comparison on Alzheimer MRI

This notebook aims to compare the performance of four Nonlinear Dimensionality Reduction (NLDR) techniques: Isometric Mapping (Isomap), Locally Linear Embedding (LLE), Diffusion Maps and t-Distributed Stochastic Neighbor Embedding (t-SNE) on an Alzheimer MRI dataset.
They are compared based on four clustering metrics: the Calinski-Harabasz Index, the Davies-Bouldin Index, the Fowlkes-Mallows Index and the Silhouette Score and on the training of a Machine Learning Classifier (Random Forest Classifier) and the assessment of the popular metrics: Accuracy, Precision, Recall and F1-score.

## Installation

### Prerequisites:

This is a Python Notebook.
Make sure you have Python installed. You can download it from the official [Python website](https://www.python.org/).

You can either use Jupyter Notebook or Google Collab.
To install Jupyter Notebook using pip:

```
pip install jupyter notebook
```

To use Google Colab, you'll need a Google account.
After that you can access [Google Colab](https://colab.research.google.com/).

### Dependencies:

You have to install the following libraries:

- Numpy
```
pip install numpy==1.26.4
```

- Pandas
```
pip install pandas==2.2.2
```

- MatPlotLib
```
pip install matplotlib==3.8.0
```

- PyDiffMap
```
pip install pydiffmap==0.2.0.1
```

### Running the Notebook Locally (Jupyter Notebook):

1. Open Jupyter Notebook:
- Open your terminal or command prompt
- Navigate to the directory where your .ipynb file is located
- Type jupyter notebook and press Enter
- This will open Jupyter Notebook in your default web browser

2. Open the Notebook:
- In the Jupyter Notebook interface, locate and click on your .ipynb file to open it

3. Run the Notebook:
- You can run individual cells or the entire notebook by using the "Run" button or keyboard shortcuts (Shift+Enter)

### Running the Notebook on Google Colab:

1. Upload the Notebook:
- Go to  [Google Colab](https://colab.research.google.com/)
- Click on "File" -> "Upload Notebook" and select your .ipynb file

2. Run the Notebook:
- You can run the notebook cell by cell or all at once using the "Runtime" menu

## Usage

To use the notebook, you must first run the imoprt cells and the cells from Data Preprocessing up to Plotting Functions.
The following sections contain the experiments witch can be rerun or adjusted. 
Each cell will display the results for the corresponding experiment, with plots and tables for each metric.

## Contributing

We welcome contributions to this notebook! Here are some hints related to how you can contribute:

- Create a fork of this repository on GitHub.
- Create a new branch for your feature or bug fix.
- Implement your changes and test them thoroughly.
- Commit your changes with clear and concise commit messages. 
- Push your branch to your forked2 repository.   
- Submit a pull request to the main repository, describing your changes and addressing any potential issues.

## License

This notebook is licensed under the [MIT License](./LICENSE). Please refer to the LICENSE file for more details.
