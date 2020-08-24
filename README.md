# ansible-k8s-ha-cluster on OpenTelekomCloud

Ansible scripts to install an kubernetes ha cluster. (draft during a training)

## Requirements

- ansible 2.9.11
- all nodes are CentOS 7

## Infrastructure example

- Masternode 01: 192.168.0.70
- Masternode 02: 192.168.0.71
- Masternode 03: 192.168.0.72
- Workernode 01: 192.168.0.80
- Workernode 02: 192.168.0.81
- Workernode 03: 192.168.0.82
- Virtual IP: 192.168.0.90

## Usage

```shell
# partial example
$ ansible-playbook kubernetes.yml -i inventory --limit kubernetes_master_nodes --tags "prerequisites"
```
