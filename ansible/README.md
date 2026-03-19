### Install
```bash
ansible-playbook ansible/play-k3s.yaml -i ansible/inventories/inventory.yaml -u ubuntu -vv
```
### Flush
```bash
ansible-playbook ansible/play-k3s.yaml -i ansible/inventories/inventory.yaml -u ubuntu -vv --extra-vars 'flush_all=true'
```