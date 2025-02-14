# Setting up Solus for devops

Solus is a rock solid Linux distro from the future. 
And this is a devops setup recap for devs like you that need get things done.

## Editors
Select the one that suits the job.

    sudo eopkg it vscode sublime-text-3 zed

## Git
    sudo eopkg it git

Configure git:

    git config --global user.name "Your Name"
    git config --global user.email "you@your-domain.com"
    git config --global color.ui auto

## JVM/Maven/Gradle
Open a terminal and install [SdkMan!](https://sdkman.io)

    > curl -s "https://get.sdkman.io" | bash

With SdkMan! installed, type following commands to install Java SDKs:

    > sdk install java
    > sdk install maven
    > sdk install gradle

Use 'sdk list' to see all SDK's and Java versions that are available.

## Docker/Minikube
    sudo eopkg it minikube

    sudo eopkg it docker docker-compose
    
To use docker without `sudo`:    
    
    sudo usermod -aG docker $USER

## Kubectl 
    sudo eopkg it kubectl

## Go
    sudo eopkg it golang
    export GOPATH="$HOME/go"
    
Add `$GOPATH/bin` to your path.

## Helm
Open a terminal and type:

    > git clone https://github.com/helm/helm.git helm
    > cd helm
    > make

Copy the build executable from '/bin'

## MongoDB

    sudo eopkg it mongodb mongo-tools

## Java IDE

Download and unzip to install [latest Eclipse](https://www.eclipse.org/downloads/packages/)
        
Download and unzip to install [Spring Tools](https://spring.io/tools)    

IntelliJ: download using the Software Installer (under Third Party) or look for AppImage or Flatpack packages.

## NodeJS

Install [NVM](https://github.com/nvm-sh/nvm?tab=readme-ov-file#installing-and-updating), the NodeJS Version Manager:

    curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.40.1/install.sh | bash

To install the latest NodeJS version, type:

    nvm install node

Type 'nvm list' to see all NodeJS versions to choose from.

## AI Tools

### Warp

Download Warp : https://www.warp.dev/download

Fix Warp ignoring `~/.bashrc` (see https://github.com/warpdotdev/Warp/issues/4722):

Add a `~/.bash_profile` file, add `source ~/.bashrc`

### Goose

See https://block.github.io/goose/docs/quickstart/

