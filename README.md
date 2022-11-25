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
where
  ```name``` is the name of your environment, use "<yourfirstname>_env"

