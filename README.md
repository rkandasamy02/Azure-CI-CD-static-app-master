# cicdapp for MLOps Project V9

## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Lints and fixes files
```
npm run lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).



# Local Setup

## To Run this py script install the below


## Install Robot Framework (https://robotframework-browser.org/)
```
pip install robotframework-browser
```

## The browser runtine required node.js
Install node dependencies.

init command is needed when library is installed or updated. When installing first time, run
```
rfbrowser init chromium
```

## Intall the PySide6 UI framework (https://pypi.org/project/PySide6/)
```
pip install PySide6
```

## Run application  in local environment
```
python pysideclient.py
```



# To make the script as executable.


## Install pyinstaller
```
pip install pyinstaller
```


## PyInstaller bundles a Python application and all its dependencies into a single package. 
```
pyinstaller --name="Sitehub-Robot_v5"  --windowed  pysideclient.py
```



# Cleanup Local Setup

```
rfbrowser clean-node
```

```
pip uninstall  robotframework-browser
```

```
pip uninstall  PySide6
```

```
pip uninstall  pyinstaller
```
