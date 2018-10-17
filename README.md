# Rancher


1 - Instalando o Servidor Ubuntu Server 16.04

2 - Instalando o Docker
    sudo curl https://releases.rancher.com/install-docker/17.03.sh | sh
    sudo usermod -aG docker $USER
    docker run hello-world
    sudo systemctl enable docker

3 - Instalando o Rancher
    docker run -d --restart=unless-stopped -p 8080:80 -p 8443:443 rancher/rancher:latest