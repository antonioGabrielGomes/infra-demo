    1  apt-get update
    2  apt-get upgrade
    3  curl
    4  apt-get install curl
    5  apt-get install git
    6  git config --global user.email 'antonio'
    7  git config --global user.name 'antonio'
    8  curl -fsSL https://get.docker.com | bash
    9  docker --version
   10  docker run hello-world
   11     curl -LO "https://dl.k8s.io/release/$(curl -L -s https://dl.k8s.io/release/stable.txt)/bin/linux/amd64/kubectl"
   12  ls
   13  mv kubectl Documents/
   14  cd Documents/
   15  ls
   16  ls -lha
   17  sudo install -o root -g root -m 0755 kubectl /usr/local/bin/kubectl
   18  kubectl version 
   19  kubectl version --client
   20  kubectl cluster-info
   21  apt-get install bash-completion -y
   22  source /usr/share/bash-completion/bash_completion
   23  echo 'source <(kubectl completion bash)' >>~/.bashrc
   24  uname -m
   25  [ $(uname -m) = x86_64 ] && curl -Lo ./kind https://kind.sigs.k8s.io/dl/v0.23.0/kind-linux-amd64
   26  ls
   27  chmod +x ./kind
   28   mv ./kind /usr/local/bin/kind
   29  kind --version
   30  git clone https://github.com/antonioGabrielGomes/infra-demo.git
   31  cd infra-demo/
   32  l
   33  ls
   34  git pull
   35  ls
   36  cd kubernetes-overview/
   37  ls
   38  cat cluter-kind.yaml 
   39  kubectl config view
   40  kubectl config get-contexts
   41  kind create cluster --name testekubernets --config cluster-kind.yaml
   42  ls
   43  mv cluter-kind.yaml cluster-kind.yaml
   44  cat cluster-kind.yaml 
   45  kind create cluster --name testekubernets --config cluster-kind.yaml
   46  kubectl config get-contexts
   47  kubectl config view
   48  nano cluster-kind.yaml 
   49  kind create cluster --name testekubernets --config cluster-kind.yaml
   50  nano cluster-kind.yaml 
   51  kind create cluster --name testekubernets --config cluster-kind.yaml
   52  kubectl cluster-info --context kind-testekubernets
   53  kubectl config view
   54  kubectl config get context
   55  kubectl config get-context
   56  kubectl config getcontext
   57  kubectl config -h
   58  kubectl config get-contexts
   59  kubectl get nodes
   60  kubectl get nodes
   61  kubectl get nodes -o wide
   62  kubectl get nodes --show-labels
   63  kubectl get nodes --show-labels
   64  kubectl config get-contexts
   65  kubectl config get-contexts --help
   66  kubectl --heĺp
   67  kubectl --help
   68  kubectl config --help
   69  kubectl config get-contexts
   70  kubectl config view
   71  history > ./lessons/lesson001.txt
   72  mkdir lessons
   73  history > /lessons/lesson001.txt
   74  history > ./lessons/lesson001.txt
   75  cat ./lessons/lesson001.txt 
   76  git add .
   77  git commit -m 'exec'
   78  git push
   79  docker ps
   80  kubectl config get-contexts
   81  ls
   82  cd Documents/
   83  ls
   84  cd infra-demo/
   85  ls
   86  cd kubernetes-overview/
   87  ls
   88  cat lessons/lesson001.txt 
   89  kubectl config view
   90  kubectl config get-contexts
   91  kubectl get nodes
   92  kubectl get nodes -o wide
   93  dd
   94  git pull
   95  ### 111 ###
   96  kubectl get namespace
   97  kubectl create -f namespace.yaml
   98  kubectl get namespace
   99  kubectl describe namespace testekubernets
  100  kubectl create -f pod.yaml
  101  cat pod.yaml 
  102  kubectl create -f pod.yaml
  103  git pull
  104  kubectl get namespace
  105  kubectl describe namespace testekubernets
  106  kubectl create -f pod.yaml
  107  kubectl get pods testekubernets
  108  kubectl get pods --namespace testekubernets
  109  kubectl describe pod nginx
  110  kubectl describe pod nginx
  111  kubectl describe pod nginx -n testekubernets
  112  kubectl get pods --namespace testekubernets
  113  kubectl describe pod nginx -n testekubernets
  114  kubectl get pods -n testekubernets
  115  kubectl port-forward pod/nginx -n testekubernets  8080:80
  116  kubectl logs -f nginx
  117  kubectl logs -f nginx -n testekubernets
  118  kubectl delete pod nginx -n testekubernets
  119  kubectl get pods -n testekubernets
  120  kubectl delete -f namespace.yaml
  121  kubectl get namespace
  122  ls
  123  history > lessons/lesson002.md
