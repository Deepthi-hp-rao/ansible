# ANSIBLE

Ansible is an open-source configuration management, software provisioning, and application deployment tool that makes automating your application deployments and IT infrastructure operation very simple.

## Ansible cmds

```
ansible --version
ansible all -i inventory_file_name --list-hosts
ansible grp_name -i inventory_file_name --list-hosts
ansible ungrouped -i inventory_file_name --list-hosts
ansible-doc -l | wc -l (to list total number of ansible modules)
ansible all -m ping (Testing Connectivity)
ansible-doc module_name(view the description of the perticular module-how to use)
ansible all -m command -a "uptime"

ansible-playbook -i inventory file_name.yaml
ansible-playbook -i inventory file_name.yml --syntax-check(check if playbook has syntax errors)
ansible-playbook -i inventory file_name.yml --check(dry run the playbook)
ansible-playbook -i inventory file_name.yml --list-hosts
ansible-playbook -i inventory file_name.yml --list-tasks
ansible-playbook -i inventory file_name.yml --tags tag_name
```
