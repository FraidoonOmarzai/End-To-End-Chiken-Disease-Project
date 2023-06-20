# End-To-End-DL-Project

## Steps

* create and activate the environment
```bash
conda create -n dl-env python=3.8 -y
conda activate dl-env
```

* create template.py to add folder structure
```bash
touch template.py
```

* define a setup.py file

* add required libraries to requirements.txt and pip install it
```bash
pip freeze
pip freeze | grep pandas
```
**Note:** The **Logging** is a means of tracking events that happen when some software runs. 
*  add code to src/cnnClassifier/__init__.py  to define logging and create test.py for test purpose

**Note:** The **utils.py** makes it easy to execute common tasks in Python scripts
* define utils (src/cnnClassifier/utils/utils.py)

```
### Workflows
1. Update config.yaml
2. Update secrets.yaml [Optional]
3. Update params.yaml
4. Update the entity
5. Update the configuration manager in src config
6. Update the components
7. Update the pipeline
8. Update the main.py
9. Update the dvc.yaml
```


****** Data Ingestion Section *******

* [Data-Link](https://github.com/FraidoonOmarzai/data/blob/main/Chicken_disease_img.zip)

* first we will run on jupyter-notebook

* add code to config.yaml ---> constants/__init__.py ---> create research/01_data_ingestion.ipynb and run it

* create entity/config_entity.py ---> configuration.py ---> components/data_ingestion.py ---> pipeline/stage_01_data_ingestion.py ---> and define main.py and run **python main.py**

