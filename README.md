# Home infrastructure
Home infrastructure scripts

## Ansible

### Create and activate virtual env (optional)
```bash
virtualenv --python="/usr/bin/python3" --clear ./venv
source ./venv/bin/activate
```

### Install ansible and tools
```bash
pip install -U ansible-core ansible ansible-lint ansible-navigator
```


### Install ansible collections and roles
```bash
cd ansible
./bin/install-ansible-roles
./bin/install-ansible-collections
```


### Run ansible playbooks
```bash
./bin/ansible-playbook init.yml
./bin/ansible-playbook node-exporter.yml
./bin/ansible-playbook docker.yml
```
