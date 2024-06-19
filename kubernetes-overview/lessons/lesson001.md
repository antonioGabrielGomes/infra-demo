Atualização e Instalação de Pacotes

    Atualização do Sistema
        apt-get update
        apt-get upgrade

    Instalação de Ferramentas
        apt-get install curl
        apt-get install git
        apt-get install bash-completion -y

Docker

    Instalação do Docker
        curl -fsSL https://get.docker.com | bash

    Verificação da Instalação do Docker
        docker --version
        docker run hello-world

Kubernetes (kubectl)

    Instalação do kubectl
        curl -LO "https://dl.k8s.io/release/$(curl -L -s https://dl.k8s.io/release/stable.txt)/bin/linux/amd64/kubectl"
        mv kubectl Documents/
        sudo install -o root -g root -m 0755 kubectl /usr/local/bin/kubectl

    Verificação da Instalação do kubectl
        kubectl version
        kubectl version --client
        kubectl cluster-info

    Autocompletar do kubectl
        source /usr/share/bash-completion/bash_completion
        echo 'source <(kubectl completion bash)' >>~/.bashrc

Kind (Kubernetes in Docker)

    Instalação do Kind
        [ $(uname -m) = x86_64 ] && curl -Lo ./kind https://kind.sigs.k8s.io/dl/v0.23.0/kind-linux-amd64
        chmod +x ./kind
        mv ./kind /usr/local/bin/kind

    Verificação da Instalação do Kind
        kind --version

Projeto de Demonstração com Kubernetes

    Clonagem de Repositório
        git clone https://github.com/antonioGabrielGomes/infra-demo.git
        cd infra-demo/

    Configuração do Cluster Kubernetes
        cd kubernetes-overview/
        cat cluster-kind.yaml
        kubectl config view
        kubectl config get-contexts
        kind create cluster --name testekubernets --config cluster-kind.yaml
        mv cluter-kind.yaml cluster-kind.yaml
        cat cluster-kind.yaml
        kind create cluster --name testekubernets --config cluster-kind.yaml
        kubectl cluster-info --context kind-testekubernets

Comandos Kubectl Adicionais

    Comandos de Configuração e Informações
        kubectl config get-contexts
        kubectl config view
        kubectl get nodes
        kubectl get nodes -o wide
        kubectl get nodes --show-labels