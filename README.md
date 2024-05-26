> This tutorial is a modified version of the original developed by [Kelsey Hightower](https://github.com/kelseyhightower/kubernetes-the-hard-way).

<<<<<<< HEAD
# Kubernetes The Hard Way On VirtualBox

This tutorial walks you through setting up Kubernetes the hard way on a local machine using VirtualBox.
This guide is not for people looking for a fully automated command to bring up a Kubernetes cluster.
If that's you then check out [Google Kubernetes Engine](https://cloud.google.com/kubernetes-engine), or the [Getting Started Guides](http://kubernetes.io/docs/getting-started-guides/).

Kubernetes The Hard Way is optimized for learning, which means taking the long route to ensure you understand each task required to bootstrap a Kubernetes cluster.
=======
This tutorial walks you through setting up Kubernetes the hard way. This guide is not for someone looking for a fully automated tool to bring up a Kubernetes cluster. Kubernetes The Hard Way is optimized for learning, which means taking the long route to ensure you understand each task required to bootstrap a Kubernetes cluster.
>>>>>>> upstream/master

This tutorial is a modified version of the original developed by [Kelsey Hightower](https://github.com/kelseyhightower/kubernetes-the-hard-way).
While the original one uses GCP as the platform to deploy kubernetes,  we use VirtualBox and Vagrant to deploy a cluster on a local machine. If you prefer the cloud version, refer to the original one [here](https://github.com/kelseyhightower/kubernetes-the-hard-way)

Another difference is that we use Docker instead of containerd. There are a few other differences to the original and they are documented [here](docs/differences-to-original.md)

> The results of this tutorial should not be viewed as production ready, and may receive limited support from the community, but don't let that stop you from learning!

## Copyright

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License</a>.


## Target Audience

The target audience for this tutorial is someone who wants to understand the fundamentals of Kubernetes and how the core components fit together.

## Cluster Details

Kubernetes The Hard Way guides you through bootstrapping a basic Kubernetes cluster with all control plane components running on a single node, and two worker nodes, which is enough to learn the core concepts.

<<<<<<< HEAD
* [Kubernetes](https://github.com/kubernetes/kubernetes) 1.13.0
* [Docker Container Runtime](https://github.com/containerd/containerd) 18.06
* [CNI Container Networking](https://github.com/containernetworking/cni) 0.7.5
* [Weave Networking](https://www.weave.works/docs/net/latest/kubernetes/kube-addon/)
* [etcd](https://github.com/coreos/etcd) v3.3.9
* [CoreDNS](https://github.com/coredns/coredns) v1.2.2

## Labs

* [Prerequisites](docs/01-prerequisites.md)
* [Provisioning Compute Resources](docs/02-compute-resources.md)
* [Installing the Client Tools](docs/03-client-tools.md)
=======
Component versions:

* [kubernetes](https://github.com/kubernetes/kubernetes) v1.28.x
* [containerd](https://github.com/containerd/containerd) v1.7.x
* [cni](https://github.com/containernetworking/cni) v1.3.x
* [etcd](https://github.com/etcd-io/etcd) v3.4.x

## Labs

This tutorial requires four (4) ARM64 based virtual or physical machines connected to the same network. While ARM64 based machines are used for the tutorial, the lessons learned can be applied to other platforms.

* [Prerequisites](docs/01-prerequisites.md)
* [Setting up the Jumpbox](docs/02-jumpbox.md)
* [Provisioning Compute Resources](docs/03-compute-resources.md)
>>>>>>> upstream/master
* [Provisioning the CA and Generating TLS Certificates](docs/04-certificate-authority.md)
* [Generating Kubernetes Configuration Files for Authentication](docs/05-kubernetes-configuration-files.md)
* [Generating the Data Encryption Config and Key](docs/06-data-encryption-keys.md)
* [Bootstrapping the etcd Cluster](docs/07-bootstrapping-etcd.md)
* [Bootstrapping the Kubernetes Control Plane](docs/08-bootstrapping-kubernetes-controllers.md)
* [Bootstrapping the Kubernetes Worker Nodes](docs/09-bootstrapping-kubernetes-workers.md)
<<<<<<< HEAD
* [TLS Bootstrapping the Kubernetes Worker Nodes](docs/10-tls-bootstrapping-kubernetes-workers.md)
* [Configuring kubectl for Remote Access](docs/11-configuring-kubectl.md)
* [Deploy Weave - Pod Networking Solution](docs/12-configure-pod-networking.md)
* [Kube API Server to Kubelet Configuration](docs/13-kube-apiserver-to-kubelet.md)
* [Deploying the DNS Cluster Add-on](docs/14-dns-addon.md)
* [Smoke Test](docs/15-smoke-test.md)
* [E2E Test](docs/16-e2e-tests.md)
* [Extra - Dynamic Kubelet Configuration](docs/17-extra-dynamic-kubelet-configuration.md)
* [Extra - Certificate Verification](docs/verify-certificates.md)
=======
* [Configuring kubectl for Remote Access](docs/10-configuring-kubectl.md)
* [Provisioning Pod Network Routes](docs/11-pod-network-routes.md)
* [Smoke Test](docs/12-smoke-test.md)
* [Cleaning Up](docs/13-cleanup.md)
>>>>>>> upstream/master
