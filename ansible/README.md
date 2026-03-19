### Install k8s
```bash
ansible-playbook ansible/playbooks/play-k3s.yaml -i ansible/inventories/inventory.yaml -u ubuntu -vv
```
### Flush k8s
```bash
ansible-playbook ansible/playbooks/play-k3s.yaml -i ansible/inventories/inventory.yaml -u ubuntu -vv --extra-vars 'flush_all=true'
```
### Install and setup nginx with TLS
```bash
ansible-playbook ansible/playbooks/setup-nginx.yaml -i ansible/inventories/inventory.yaml -u ubuntu -v
```