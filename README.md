# Spatial Data Science
**Spring 2025**

[Remote Sensing & Spatial Analytics (RSA) Lab](https://sites.google.com/itu.edu.pk/rsa-lab/)


This a guideline on how to set up a conda environment, with the requisite packages, for the Spatial Data Science course. Please follow this instructions below.


## Set up & Activate a Conda environment

To set up and activate a new conda environment, you can use the following commands. Replace `your_environment_name` with the desired name for your new environment:

- Create a new conda environment, by calling the following at your command-prompt/terminal.


```bash
conda create --name your_environment_name
```

You can also specify a particular Python version when creating the environment:

```bash
conda create --name your_environment_name python=3.9
```

- Activate the conda environment:

```bash
conda create --name your_environment_name python=3.9
```

After activation, your command prompt or terminal prompt should change to show the active environment.

Remember to replace `your_environment_name` with the actual name you want for your environment.

## Install the libraries

You're provided with a file that contains the required libraries for this course. These libraries are:

```
pandas
numpy
geopandas
rioxarray
xarray
...

```

Place the `requirements.txt` file at any conveninent directory; a good idea is to set up a separate directory for all the code related to this course.  Please run the following command, after switching the prompt to that directory.

```bash
pip install -r requirements.txt
```

Normally, this should be fine, but if you run into some version conflicts, please let me know. During this process, the terminal will prompt you to confirm the installations. Please proceed. Several dependencies will automatically be installed alongside, such as the libraries `fiona`, `gdal`, etc. These libraries may also be used during the course.

General help regarding conflicts: At times, conflicts be resolved by breaking the install into smaller steps. First check the library that raised an error, and ascertain which requirement is unfulfilled. For example, if it says that `numpy` (or a certain version thereof) is required, just install it while removing the previous cache (during failed installation).

```bash
pip install --no-cached-dir numpy
```

Install other libraries step up step. Carefully watch for any breaks, and assess the conflict. The way around the conflict might be system specific (and can depend on the global installs previously made/available on your system).




