# treehacks-2024
## InterSystems IRIS Quickstart

dataset from https://www.kaggle.com/datasets/koki25ando/22000-scotch-whisky-reviews

1. Clone the repo
    ```
    https://github.com/alvin-isc/treehacks-2024.git
    ```
    In the following steps, replace 'PATH' with the path to the repo. 
2. Install IRIS (Community Edtion) in a container:
    ```
    docker run --name iris -d --publish 1972:1972 --publish 52773:52773 containers.intersystems.com/intersystems/iris-community-arm64:latest-preview 
    ```
    - Access the System Management Portal via http://localhost:52773/csp/sys/UtilHome.csp (user: SUPERUSER, pw: SYS)
    - Change the password as prompted
3. Create a python environment (conda, venv or however you wish) For example:
    
    ```
    conda create --name treehacks-iris python=3.10
    ``` 
    
## Install packages for all demos:
```
pip install -r requirements.txt
```

## Install packages for specific demos:
### sql_demo.ipynb:
```
 pip install 
```

### langchain_demo.ipynb:
```
 pip install 
```

### llama-demo.ipynb: