# RStudio and Radian Docker Image for Codespace

This repos provides the image based on `rocker/tidyverse` that can be directly used by codespace of Github.

This docker image is re-published every week on [https://hub.docker.com/r/rickyking/codespace-rstudio](). 

Features:

- full `tidyverse` installed
- `RStudio Server` available to be accessed via port forward
- `radian` installed for better VS Code compability

## How to setup the codespace-rstudio

Step 1: create a github repo and lauch default codespace

Step 2: in the codespace web or local vscode, create following stucture

```
├── .devcontainer
│   ├── devcontainer.json
│   └── Dockerfile
└── README.md
```

Step 3: copy paste the content of [devcontainer.json](devcontainer.json)

Step 4: in `Dockerfile`, just put `FROM rickyking/codespace-rstudio`

## TODO
