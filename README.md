# Kubernetes install on Raspberry Pi with Ansible

This repo holds the files to install a real kubernetes cluster to multiple RPI
The goal of this automation is to simulate an cluster as real to production as possible on RPI

We will not be using k8s or minikube or any of the other available solutions, as they tend to have certain features removed.
They work great if you quickly need a cluster, but for long term running and experimentation, you will feel this.
I know i did.

## pre-requirements
* raspberry pi's model 4 (8GB preferred) -> SD card is fine -> USN nvme is better
* 3 x controllers + Xn x workers nodes -> mine is 3 controllers + 5 workers
* Install Ubuntu:21.04 on all of them (21.04 is needed to have working usb boot, with no problems during updates)

install ansible from the requirements file not the packaged version from your OS, as they tend to be old.
