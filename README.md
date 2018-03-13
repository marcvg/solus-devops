# solus-devops
Solus Devops setup guide

## Git/Maven
    eopkg it git apache-maven

Configure git:

    git config --global user.name "Your Name"
    git config --global user.email "you@your-domain.com"
    git config --global color.ui auto

## Docker/Minikube
    eopkg it minikube virtualbox-common

    eopkg it docker docker-compose
    
To use docker without `sudo`:    
    
    sudo usermod -aG docker $USER

## Kubectl 
    sudo snap install kubectl

## Go
    eopkg it golang
    export GOPATH="$HOME/go"
    
Add `$GOPATH/bin` to your path.

