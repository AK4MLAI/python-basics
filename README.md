# PythonBasics

## Setup the virtual environment using conda
### Register conda with git bash
To register conda in git bash, create or edit the file .bashrc (C:\Users\ambarishk) and add this line
. /c/installer/anaconda3/etc/profile.d/conda.sh

### Create conda virtual environment
1) open git bash from the project (/c/MyLearning/Python)
2) conda create -n my-env python=3.13.9
3) conda activate my-env
4) pip install jupyter pandas numpy matplotlib
5) pip install transformers torch scikit-learn

### Register environment in jupyter
1) pip install ipykernel
2) python -m ipykernel install --user --name=my-env --display-name "Python 3 (my-env)"

### Open the notebook
1) open git bash from the project (/c/MyLearning/Python)
2) conda activate my-env
3) jupyter notebook

## Delete the virtual environment
1) conda deactivate
2) conda remove --name my-env --all
3) conda env list

### Deregister environment in jupyter
1) jupyter kernelspec uninstall my-env
2) jupyter kernelspec list

