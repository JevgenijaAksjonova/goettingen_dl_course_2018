# Göttingen DL course material

This is the repository for course material (input and output) for the "Mathematics of deep learning with an emphasis on inverse problems" course at Göttingen 2018.

## Setting up the environment

Install anaconda by following official installation instructions at
https://www.anaconda.com/products/individual

It should look similar to the following commands, but with different software versions  

   $ wget https://repo.anaconda.com/archive/Anaconda3-5.2.0-Linux-x86_64.sh \
   $ chmod  +x Anaconda3-5.2.0-Linux-x86_64.sh \
   $ ./Anaconda3-5.2.0-Linux-x86_64.sh 

Create a new environment named "myenv" by 

   $ conda create -n myenv python=3.10

Activate this environment

   $ conda activate myenv

Install pytorch 

   $ conda install -c pytorch pytorch torchvision

Install back-ends for odl

   $ conda install -c astra-toolbox/label/dev astra-toolbox \
   $ conda install -c anaconda scikit-image

Install odl from source 

   $ git clone https://github.com/odlgroup/odl \
   $ cd odl \
   $ pip install --editable . 

Install other packages 

   $ conda install matplotlib jupyter ipykernel

Install jupyter and make your environment visible in the jupyter notebook

   $ python -m ipykernel install --user --name myenv --display-name="My Env"
