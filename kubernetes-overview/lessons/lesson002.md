Comandos kubectl
Configuração

    kubectl config view
    kubectl config get-contexts

Nodes

    kubectl get nodes
    kubectl get nodes -o wide

Namespaces

    kubectl get namespace
    kubectl create -f namespace.yaml
    kubectl describe namespace testekubernets
    kubectl delete -f namespace.yaml

Pods

    kubectl create -f pod.yaml
    kubectl get pods testekubernets
    kubectl get pods --namespace testekubernets
    kubectl describe pod nginx
    kubectl describe pod nginx -n testekubernets
    kubectl port-forward pod/nginx -n testekubernets 8080:80
    kubectl logs -f nginx
    kubectl logs -f nginx -n testekubernets
    kubectl delete pod nginx -n testekubernets
    kubectl get pods -n testekubernets
