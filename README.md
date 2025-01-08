# NLDR Comparison on Alzheimer MRI

This notebooks aim to compare the performance of four Nonlinear Dimensionality Reduction (NLDR) techniques: Isometric Mapping (Isomap), Locally Linear Embedding (LLE), Diffusion Maps and t-Distributed Stochastic Neighbor Embedding (t-SNE) on an Alzheimer MRI dataset and help improve the accuracy of classification.
The algorithms are compared based on four clustering metrics: the Calinski-Harabasz Index, the Davies-Bouldin Index, the Fowlkes-Mallows Index and the Silhouette Score and on the training of a Machine Learning Classifier (Random Forest Classifier) and the assessment of the popular metrics: Accuracy, Precision, Recall and F1-score.
The best results are further compared based on different classification machine learning algorithms.

## Installation

### Prerequisites:

These are Python Notebooks.
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

The first notebook, 'NLDR_Comparison_MRI' is used to compare the four NLDR algorithms based on the metrics previously mentioned.
Its aim is to study which are the best parameters and which techinque has the best results.
To use this notebook, you must first run the import cells and the cells from Data Preprocessing up to Plotting Functions.
The following sections contain the experiments witch can be rerun or adjusted. 
Each cell will display the results for the corresponding experiment, with plots and tables for each metric.

The second notebook, 'NLDR_Comparison_Classification' is used to further study the best NLDR results from the first notebook.
Its aim is to train different classification algorithms on the reduced dataset and compare the results.
To use this notebook, you must first run the import cells, the cells from Data Preprocessing and those for applying the NLDR techniques.

## Contributing

We welcome contributions to this notebook! Here are some hints related to how you can contribute:

- Create a fork of this repository on GitHub.
- Create a new branch for your feature or bug fix.
- Implement your changes and test them thoroughly.
- Commit your changes with clear and concise commit messages. 
- Push your branch to your forked2 repository.   
- Submit a pull request to the main repository, describing your changes and addressing any potential issues.

## Week 10 Update

This week, we added a new notebook, 'NLDR_Comparison_Classification', which we will use to implement the second set of exeriments from the literature.
For now, we added some of the imports we need to use, we loaded our dataset and applyed the NLDR techniques on it.
Apart from this, we updated some parts of the README file to talk about the newly introduced notebook and its contents.

## Week 11 Update (Delayed from December)

This week we created functions that will help us to train different ML models with the transformed data we get from the NLDR algorithms we applied.
These functions gerenrate training/test splits of the data, predict based on an ML model, scale data (for SVM), load and train ML models, perform parameter tuning and train ML models on each data created with NLDR and plot the results (accuracy, precision, recall, f1-score).

## Week 13 Update

This week we trained three ML Classification models (Logistic Regression, Support Vector Machines and Random Forest) on the dataset transformed by our NLDR techniques. 
We plotted the accuracy, precision, recall and F1-score and desplayed the results in tables for easier analysis.

## License

This notebook is licensed under the [MIT License](./LICENSE). Please refer to the LICENSE file for more details.
