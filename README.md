# Conda in Environmental Programming
This is a quick introduction to managing your python environments for IUPWARE programmers. 

Note that arrows imply input when you use these commands ("<>"), don't include them!

## Check your environments

Open your anaconda prompt.

See what environments you have already installed:
```
conda env list
```

Note the name in brackets beside your current directory ("base"). What does this mean?

## Create a new environment

Don't type the arrows:
```
conda create -n <name> -c <channel> python=<version> <packages>
```
where,

    - "name" is the name of your environment, use "<yourfirstname>_env"
    - "channel" is the name of the channel you're retrieving packages from, use "conda-forge"  
    - "version" is the version of python you want, for now use "3.9"
    - "packages" should be a space-delimited list of package names, pick some from numpy, scipy, pickle, matplotlib, pandas, xarray
    

## Activate your environment

Try:
```
conda activate <name>
```

Check what was installed (why are there other packages in your environment in addition to the ones you called for in the conda command?):
```
conda list
```

Install some additional packages (e.g., numpy, pandas, xarray, matplotlib, seaborn, scipy).
Go to your web browser of choice type a package you haven't installed yet and type _package name conda forge_, the first result will be the one you need [for example](https://anaconda.org/conda-forge/scipy). Copy the install command and paste it into your anaconda prompt.

Check your list of environments again.


## Export your environment to a yml file, share it and install one that you receive

Make sure your environment is activated.

Create the yml file:
```
conda env export > <filename.yml>
```

Email the file to a neighbour. Install the one that a neighbour gave to you.

