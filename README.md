# treehacks-2024
## InterSystems IRIS Quickstart


1. Clone the repo
    ```
    https://github.com/alvin-isc/treehacks-2024.git
    ```
    In the following steps, replace 'PATH-TO-REPO' with the path to the repo. 
2. Install IRIS (Community Edtion) in a container:
    ```
    docker run -d --name iris-comm \
    -p 1972:1972 \
    -p 52773:52773 \
    --volume /Users/aryanput/dp/treehacks-2024/external:/external \
    containers.intersystems.com/intersystems/iris-community-arm64:2024.1-preview \
    --key /external/iris.key 
    ```
    - Access the System Management Portal via http://localhost:52773/csp/sys/UtilHome.csp (user: SUPERUSER, pw: SYS)
    - Change the password as prompted. The demo notebooks use a password of 'SYS2'.
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