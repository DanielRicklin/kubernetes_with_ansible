Check https://spacelift.io/blog/ansible-kubernetes

```
ansible-playbook playbook/kube_dependencies.yaml -i inventory.yaml
ansible-playbook playbook/kube_master.yaml -i inventory.yaml
ansible-playbook playbook/kube_workers.yaml -i inventory.yaml
```

```
ansible-playbook playbook/test_deployment.yaml -i inventory.yaml
ansible-playbook playbook/test_delete_deployment.yaml -i inventory.yaml
```