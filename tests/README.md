# Data Team Project Template #
## Overview ##
* Quick summary
* Version
* [Learn Markdown](https://bitbucket.org/tutorials/markdowndemo)

## Configuration ##

### Creating a Project

```
poetry new <project_name>
```

#### In an existing folder 

```
poetry init
```

### Set Python Environment 

We use `python3.8`. 

```
poetry env use python3.8
```

#### For `scipy` edit `pyproject.toml` for specific python version

`python` property to ">=3.8,<3.12"

```
[tool.poetry.dependencies]
python = ">=3.8,<3.12"
```

### Activate the Virtual Env 

```
poetry shell 
```
### Run Python in Virutal Env

```
poetry run python 
```

### Add Dependencies

#### Simple method

```
poetry add <package Name>
```

#### Migrating from `requirements.txt` 

```
poetry add $(cat requirements.txt)
```

### Install and Update project

```
poetry install
poetry update
```

### To run test 

```
poetry run pytest
```

### For updating poetry itself

```
poetry self update
```

### Building `whl` and `tar` files


```
poetry build 
```

### Confirm the environment variables

```
poetry env info
```

### Export `requirements.txt` 

```
poetry export --without-hashes --format=requirements.txt > requirements.txt
```



## Project Specific Configuration ##
* Summary of set up
* Configuration
* Dependencies
* Database configuration
* How to run tests
* Deployment instructions

## Project Details ##

* Writing tests
* Code review
* Other guidelines

## Remaining issue

* Enable folder creation upon creation (`data`, `notebooks`, etc)
* Add git repo information in pyproject.toml
* Add documentation for `pytest` 
* Import/Export `environment.yml` for conda
* Dockerfile integration

