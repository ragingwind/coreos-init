# CoreOS Initialing Tools - Raw level

## git-init

Create a target repo for bare git and you can register a shell command to get event from `post-receive` event of git when if git got new commits.

    git-init [TARGET_REPO_PATH] [POST_RECEIVE_EVENT_HANDLER]
    
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


