# DS--cleancode_structure
This repository lists the steps to launch a clean code structure for your data science or data analysis project. Each tool used will be described by its main utility.

1. Create a conda environment for your project in your destination folder :
```
C:\Users\Ybenallal\Documents\clean_code> conda create -n exampleproject python=3.9
```
2. Activate your conda environment :
```
C:\Users\Ybenallal\Documents\clean_code> conda activate exampleproject
```
3. Install cookiecutter :
```
(exampleproject) C:\Users\Ybenallal\Documents\clean_code>pip install cookiecutter
```
4. Create a project based on a template (you will be asked to fill project_name - authorname...) :
```python
(exampleproject) C:\Users\Ybenallal\Documents\clean_code>cookiecutter https://github.com/khuyentran1401/data-science-template --checkout dvc-poetry
directory_name [project-name]: myproject
author_name [Your Name]: youssef595
compatible_python_versions [^3.8]:
```
-----> This will create the following code structure (the tools used will be explained below)
![image](https://github.com/youssef595/DS--cleancode_structure/assets/56879680/adf29b05-07ab-4e29-8322-0b1244bb3397)

