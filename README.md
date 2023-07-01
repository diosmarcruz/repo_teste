# repo_teste
## atualizar pacotes
'''
sudo apt update
'''
## Instalando git
'''
sudo apt install git
'''
## verificar instalação
'''
git --version
'''
## Instalando git flow
'''
sudo apt install git-flow
'''
### verificar instalação
'''
git-flow --version
'''
## Instalando gh
'''
sudo apt install gh
'''
## verificar instalação
'''
gh --version
'''
## Instalando o Docker

## Link de Instalação https://docs.docker.com/engine/install/ubuntu/

nstall using the apt repository

Before you install Docker Engine for the first time on a new host machine, you need to set up the Docker repository. Afterward, you can install and update Docker from the repository.
Set up the repository

    # 1 Update the apt package index and install packages to allow apt to use a repository over HTTPS:
    '''
    sudo apt-get update
    '''
    sudo apt-get install ca-certificates curl gnupg
    '''
    
# 2 Add Docker’s official GPG key:
'''
sudo install -m 0755 -d /etc/apt/keyrings
 curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /etc/apt/keyrings/docker.gpg
 '''
 sudo chmod a+r /etc/apt/keyrings/docker.gpg
'''
 # 3 Use the following command to set up the repository:
 '''
 echo \
  "deb [arch="$(dpkg --print-architecture)" signed-by=/etc/apt/keyrings/docker.gpg] https://download.docker.com/linux/ubuntu \
  "$(. /etc/os-release && echo "$VERSION_CODENAME")" stable" | \
  sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
'''
  ## Install Docker Engine
  # 1 Update the apt package index:
  '''
  sudo apt-get update
'''
  # To install the latest version, run:
  '''
  sudo apt-get install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin
'''
  # Verify that the Docker Engine installation is successful by running the hello-world image.
'''
  sudo docker run hello-world
'''

  
    
