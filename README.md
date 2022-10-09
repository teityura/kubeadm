# kubeadm

## Define hosts

```
vim hosts.ini
vim group_vars/all.yml
```

## Setup all

```
ansible-playbook site.yml -vv
```

## Setup ssh

```
ansible-playbook site.yml -t ssh,user -vv
```

## Initialize k8s cluster

```
ansible-playbook site.yml -t kubeadm-init -vv
```

## Delete k8s cluster

```
ansible-playbook site.yml -t kubeadm-delete -vv
```

