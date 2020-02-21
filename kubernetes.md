# Kubernetes
See also https://kubernetes.io/docs/reference/kubectl/cheatsheet/

* `kubectl cp /local_dir <k8s-namespace>/<pod-name>:/destination`: copy from local disk to destination. Reverse for the oposite action.
* `kubectl top nodes`: Top on nodes.
* `sudo kubectl top pods --all-namespaces`: Top on pods.
* `kubectl get pods | grep Evicted | awk '{print $1}' | xargs kubectl delete pod`: delete all envicted pods (example from https://gist.github.com/zparnold/0e72d7d3563da2704b900e3b953a8229)

# Minikube
* `sudo cp /run/systemd/resolve/resolv.conf /etc/resolv.conf`: Replace local dns config (*More info to be added*).

# Helm
See also https://helm.sh/docs/intro/using_helm/

* `helm install ...`: ...
* `helm uninstall ...`: ...
* `helm list --all`: ...

# Extras:
* https://crontab.guru/
