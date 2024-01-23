AMLS II
=======

This code is for use within the UCL Electronic Engineering AMLS II module (ELEC0135).

Setup
-----
**Please use Google Colab to run the code.**


**You should start with the following steps:**

Open the .ipynb file that you would like to run in GitHub. 
Then, in the URL above, change **github.com** to **githubtocolab.com** and press Enter.

In the first cell, clone this GitHub project, and run::

    !git clone https://github.com/cwfparsonson/AMLS_II
    
Go to the directory where the file you initially opened is saved, using %cd.

For example::
    If you opened the file Lab1_MLP.ipynb initially.
    You add a code line at the top of the code to clone the repository.
    Then, you add a new code cell that you use to enter the corresponding directory, %cd AMLS_II/Lab1/Lab1_MLP/
    
Now, in a new cell at the top of the code, run the following lines to install the needed packages::
    
    For Lab2:
        !pip install --upgrade tf_slim


Issues
------
The following issues have previously been encountered and resolved:

- **Problems with dlib**: For ``dlib==19.16.0`` to install, you may need to separately install ``cmake``
  by running ``python -m pip install cmake``. For ``cmake`` to work, you may also need to install
  a C++ compiler with ``sudo apt-get install g++`` (Linux). You should then be able to run
  ``python -m pip install dlib==19.16.0``

- **Jupyter accessing environment**: For your environment to be selectable as a kernel in Jupyter Notebook, once you
  have installed the required packages into your virtual environment called ``<env_name>``,
  you may need to run ``python -m ipkykernel install --user --name <env_name> --display-name "<env_name>"``
  so that you can select your ``<env_name>`` in the Jupyter Notebook under Kernel -> Change kernel -> ``<env_name>``.

- **Linux memory errors**: If you are partitioning your drive to run Linux, you may encounter tmp memory errors
  when installing the ``requirements.txt`` file. To solve this, you will need to free up swap memory
  on your Linux machine so the packages can be installed: https://askubuntu.com/questions/178712/how-to-increase-swap-space

If you have any questions or issues, please do not hesitate to raise a GitHub issue 
on this AMLS_II repository. To raise an issue, at the top of the window at https://github.com/cwfparsonson/AMLS_II,
go to Issues -> New issue, and fill out your post. We will answer your issues/questions ASAP.
