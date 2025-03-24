# NGS Bioinformatics Analysis

This project focuses on mapping out cell types using clustering and UMAP bioinformatics analysis. It leverages single-cell RNA sequencing (scRNA-seq) data to identify distinct cell populations.

## 🧬 Project Overview
This project analyzes **single-nucleus RNA sequencing (snRNA-seq) data** from the **GSE138852 dataset**, which focuses on **Alzheimer's disease**. The goal is to map out **cell types** in the **entorhinal cortex** and study how **gene expression changes** in different cell subpopulations contribute to the disease.

### **Key Features**
- **Data Processing:** Reads and processes gene expression data from `GSE138852_counts.csv` and metadata from `GSE138852_covariates.csv`.
#### 🧬 Data Preprocessing
1. **Doublet Elimination**: Remove doublets to ensure accurate results.
2. **Quality Control**: Filter cells with low gene counts, high mitochondrial content, and low gene expression.
3. **Normalization**: Normalize data to account for sequencing depth differences.
4. **Log Transformation**: Prepare data for clustering and visualization.
5. **Visualize QC Metrics**: Optionally use violin plots to check data distributions.

#### 🧬 Data Analysis tools
- **Dimensionality Reduction:** Uses **UMAP** for visualization.
- **Clustering:** Identifies different cell populations using **Scanpy**, **Leiden clustering**, and **scVI-tools**.
- **Gene Expression Analysis:** Examines how the **APOE gene**, a known risk factor for Alzheimer's, is differentially expressed in **oligodendrocyte progenitor cells**, **astrocytes**, and **microglia**.
- **Machine Learning:** Uses **silhouette scores** and **nearest neighbor analysis** for clustering validation.

## 🛠 Technologies Used
- **Python**: Main programming language.
- **Scanpy**: Single-cell analysis framework.
- **Pandas**: Data manipulation.
- **Scivi-tools**: Advanced single-cell analysis tools.
- **PyTorch**: Deep learning framework.
- **UMAP**: Nonlinear dimensionality reduction.
- **Leiden Algorithm**: For clustering.
- **Seaborn & Matplotlib**: Data visualization.

## 📂 Dataset
The project uses an Alzheimer's disease scRNA-seq dataset from GEO: **GSE138852**. 

## 🚀 Installation
To set up the environment and run the analysis:

1. Clone the repository:
   ```bash
   git clone https://github.com/PAS195Pitt/NGS-Bioinf-Basic.git
   cd NGS-Bioinf-Basic
   ```

2. Create and activate a virtual environment (optional but recommended):
   ```bash
   python -m venv venv
   source venv/bin/activate   # On Windows use: venv\Scripts\activate
   ```

3. Install required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Run the Jupyter Notebook:
   ```bash
   jupyter notebook NGS.ipynb
   ```

## 📌 Future Improvements
- Improve clustering techniques for better resolution.
- Apply deep learning models to refine cell type classification.
- Optimize computational efficiency for large datasets.


### ✉️ Contact
For any questions or contributions, feel free to reach out!

