# Rancher

## Bedingung
1) Laufender DNS, für das Load-Ballancing

Fragestellung ob Lightweight => k3s oder Full RKE(Rancher Kubernetes Engine)


RKE
Rancher Kubernetes Engine (RKE) is a CNCF-certified Kubernetes distribution that runs entirely within Docker containers. It works on bare-metal and virtualized servers. RKE solves the problem of installation complexity, a common issue in the Kubernetes community. With RKE, the installation and operation of Kubernetes is both simplified and easily automated, and it’s entirely independent of the operating system and platform you’re running. As long as you can run a supported version of Docker, you can deploy and run Kubernetes with RKE.


K3S
K3s is a fully compliant Kubernetes distribution with the following enhancements:

An embedded SQLite database has replaced etcd as the default datastore. External datastores such as PostgreSQL, MySQL, and etcd are also supported.
Simple but powerful “batteries-included” features have been added, such as: a local storage provider, a service load balancer, a Helm controller, and the Traefik ingress controller.
Operation of all Kubernetes control plane components is encapsulated in a single binary and process. This allows K3s to automate and manage complex cluster operations like distributing certificates.
In-tree cloud providers and storage plugins have been removed.
External dependencies have been minimized (just a modern kernel and cgroup mounts needed). K3s packages required dependencies, including:
containerd
Flannel
CoreDNS
Host utilities (iptables, socat, etc)