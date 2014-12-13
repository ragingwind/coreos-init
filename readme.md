# CoreOS Initialing Tools - Raw level

## git-init-bare-info

Create a target repo and init git with bare option for serving then add shell command to delegate post-receive hooks service of git

    git-init-base [TARGET_REPO_PATH] [SHELL_COMMAND]
    
### Usage
    
    git-init-bare ../project 'docker run -i -d --name node /dockerfile/node'

## docker-build

docker build shortcut

    docker-build [TARGET] [DOCKERFILE]

### Usage
    
    docker-build node /dockerfile/node

## docker-rerun

docker re-run shorcut. Run docker after stop and rm a target container. You can pass Docker Volume params conf to command
    
    docker-rerun [NAME] [PORTS STRING] [VOLUME PARAMS FILE PATH:OPT]

### Usage

    docker-rerun nodeapp '-p 80:80' /vparams/nodeapp


