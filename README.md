# CarDEC (by jlakkis)

Original repository: [jlakkis/CarDEC](https://github.com/jlakkis/CarDEC)

CarDEC (**C**ount **a**dapted **r**egularized **D**eep **E**mbedded **C**lustering) is a joint deep learning computational tool that is useful for analyses of single-cell RNA-seq data. CarDEC can be used to:

1. Correct for batch effect in the full gene expression space, allowing the investigator to remove batch effect from downstream analyses like psuedotime analysis and coexpression analysis. Batch correction is also possible in a low-dimensional embedding space.
2. Denoise gene expression.
3. Cluster cells.

## Citation

Lakkis, J., Wang, D., Zhang, Y., Hu, G., Wang, K., Pan, H., ...Li, M. (2021). A joint deep learning model enables simultaneous batch effect correction, denoising, and clustering in single-cell transcriptomics. Genome Res., 31(10), 1753–1766. [doi: 10.1101/gr.271874.120](https://doi.org/10.1101/gr.271874.120)

To find code to reproduce the results generated in that paper, please visit this separate [github repository](https://github.com/jlakkis/CarDEC_Codes), which provides all code (including that for other methods) necessary to reproduce the results.

## Installation

Recomended installation procedure is as follows. 

1. Install [Anaconda](https://www.anaconda.com/products/individual) (or [miniconda](https://docs.conda.io/en/latest/miniconda.html)) if you do not already have it. 
2. Create a conda environment, and then activate it as follows in terminal.

```
$ conda create -n cardecenv
$ conda activate cardecenv
```

3. Install an appropriate version of python.

```
$ conda install python=3.10
```

4. Install nb_conda_kernels so that you can change python kernels in jupyter notebook.

```
$ conda install nb_conda_kernels
```

5. Finally, install CarDEC.

```
$ pip install https://github.com/argearriojas/CarDEC.git
```

Now, to use CarDEC, always make sure you activate the environment in terminal first ("conda activate cardecenv"). And then run jupyter notebook. When you create a notebook to run CarDEC, make sure the active kernel is switched to "cardecenv"

## Usage

A [tutorial jupyter notebook](https://drive.google.com/drive/folders/19VVOoq4XSdDFRZDou-VbTMyV2Na9z53O?usp=sharing), together with a dataset, is publicly downloadable.

## Software Requirements
    
- Python >= 3.7
- TensorFlow >= 2.0.1
- scikit-learn >= 0.22.2.post1
- scanpy >= 1.5.1
- leidealgn >= 0.9.1
- pandas >= 1.0.1
- scipy >= 1.4.1

