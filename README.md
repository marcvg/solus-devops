# solus-devops
Solus Devops setup guide

## Git/Maven
    eopkg it git apache-maven 

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

