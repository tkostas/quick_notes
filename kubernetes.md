# Kubernetes
See also https://kubernetes.io/docs/reference/kubectl/cheatsheet/

* `kubectl cp /local_dir <k8s-namespace>/<pod-name>:/destination`: copy from local disk to destination. Reverse for the oposite action.
* `kubectl top nodes`: Top on nodes.
* `sudo kubectl top pods --all-namespaces`: Top on pods.

# Minikube
* `sudo cp /run/systemd/resolve/resolv.conf /etc/resolv.conf`: Replace local dns config (*More info to be added*).

# Helm
See also https://helm.sh/docs/intro/using_helm/

* `helm install ...`: ...
* `helm uninstall ...`: ...
* `helm list --all`: ...

# Extras:
* https://crontab.guru/
