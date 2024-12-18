# Modelling
`Creation` => `Training` => `Evaluation` => `Export`

## How to load dataset?
```!mkdir {HOME}/datasets
%cd {HOME}/datasets

from roboflow import Roboflow

ROBOFLOW_API_KEY = userdata.get('ROBOFLOW_API_KEY')
rf = Roboflow(api_key=ROBOFLOW_API_KEY)
project = rf.workspace("project-zero").project("aerial_river_plastic_wastes")
version = project.version(10)
dataset = version.download("yolov8")
```
`Note`: If you want dataset in the particular format to train, you have to contact me for that because it is in Roboflow Cloud Storage.

### Folders
- Script- For python scripts
- Notebook - For jupyter notebooks

    
    


