# k8s_consul

Stands up a `consul` cluster in kubernetes.

The `install-consul.sh` script stands up 3 consul servers in namespaces consul-1, consul-2 and consul-3. It waits for the pod in consul-1 to be running before it starts the ones in consul-2 and consul-3 (it has to wait for an IP address to be available for pod in consul-1).
