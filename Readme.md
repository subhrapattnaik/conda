Open google-->serach for How to manage Conda Environment


https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html#

From the Anaconda Terminal,Type the below commands

-----------------------------------------------------
conda list

pip list
---------------------------------------------------------
conda install pandas numpy matplotlib

conda remove pandas numpy matplotlib

-----------------------------------------------
pip install pandas numpy matplotlib

pip uninstall pandas numpy matplotlib
--------------------------------------------------
python -- version
ex: 3.9.12

create a new environment

conda create -n testenv2 python=3.9.12

conda activate testenv2

conda env list
------------------------------------------------

pip list

pip freeze

-----------------------------------------------
sometimes all the needed modules will be given in a file ,for ex: packages.txt
-----------------
touch packages.txt

pandas
numpy
matplotlib


ESC, :wq

---------
pip install -r packages.txt

All packages will be installed
-----------------------------------------------

Removing any virtual environment

conda remove --name testenv2 --all

where "testenv2" is the env we want to remove

------------------------------------------

conda deactivate testenv3

---------------------------

Export your env to a .yml file

conda env export > environment.yml
--------------------------------
cat environment.yml

----------------------

Sometimes you get .yml file
out of it you have to create a environment


conda env create -f environment.yml

conda activate testenv3

conda list

----------------------------------------

