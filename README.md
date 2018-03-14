# solus-devops
Solus Devops setup guide

## Editors
Select the one that suits the job.

    sudo eopkg it atom vscode sublime-text-3 

## Git/Maven
    sudo eopkg it git apache-maven

Configure git:

    git config --global user.name "Your Name"
    git config --global user.email "you@your-domain.com"
    git config --global color.ui auto

## Docker/Minikube
    sudo eopkg it minikube virtualbox-common

    sudo eopkg it docker docker-compose
    
To use docker without `sudo`:    
    
    sudo usermod -aG docker $USER

## Kubectl 
    sudo snap install kubectl

## Go
    sudo eopkg it golang
    export GOPATH="$HOME/go"
    
Add `$GOPATH/bin` to your path.

## MongoDB

    sudo eopkg it mongodb mongo-tools

## Eclipse/Spring Tools Suite

Download and unzip to install Eclipse Neon:
    http://download.springsource.com/release/ECLIPSE/oxygen/2/eclipse-jee-oxygen-2-linux-gtk-x86_64.tar.gz
        
Download and unzip to install Spring Tool Suite:    
    http://download.springsource.com/release/STS/3.9.2.RELEASE/dist/e4.7/spring-tool-suite-3.9.2.RELEASE-e4.7.2-linux-gtk-x86_64.tar.gz

