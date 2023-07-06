# DS--cleancode_structure
This repository lists the steps to launch a clean code structure for your data science or data analysis project. Each tool used will be described by its main utility.

### A. SETUP :
1. install cookiecutter :
```
C:\Users\Ybenallal>pip install cookiecutter
```
2. Navigate into your project folder and create a project based on a template (you will be asked to fill project_name - authorname...) :
```python
(exampleproject) C:\Users\Ybenallal\Documents\clean_code>cookiecutter https://github.com/khuyentran1401/data-science-template --checkout dvc-poetry
directory_name [project-name]: myproject
author_name [Your Name]: [youssef595]
compatible_python_versions [^3.8]:
```
-----> This will create the following code structure (the tools used will be explained below)
![image](https://github.com/youssef595/DS--cleancode_structure/assets/56879680/adf29b05-07ab-4e29-8322-0b1244bb3397)

### B. TOOLS:

#### B.1 poetry:
1. install poetry:
```
C:\Users\Ybenallal>pip install poetry
```
2. Activate a new environment:
```
C:\Users\Ybenallal\Documents\clean_code\mytemplate>poetry shell
```
3. To install dependancies or to install specific library, or to remove specific library:
```
C:\Users\Ybenallal\Documents\clean_code\mytemplate>poetry install
```
- After this step, a poetry.loc file(package version registry) will be created in you project.
```
C:\Users\Ybenallal\Documents\clean_code\mytemplate>poetry add <library>
```
```
C:\Users\Ybenallal\Documents\clean_code\mytemplate>poetry remove <library>
```
###### Now why poetry?
1-Adaptation to newer releases : it stores the flexible versions of packages in the tomfile
2-Reproducibility : stores the exact package version and its dependancies in poetry.lock
3-Conflicts resolving

#### B.2 pre-commit:
![image](https://github.com/youssef595/DS--cleancode_structure/assets/56879680/22e61c62-c4a4-42cb-ab3f-774620f8fbbb)
This is managed via the yaml file above (it uses ruff (fast python linter), and interrogate (checks missing docstrings))
whenever you do "git commit -m 'message'" the checks will be launched.

#### B.3 makefile:



