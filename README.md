# Home infrastructure
Home infrastructure scripts

## Ansible

Everything of the above needs to be run inside `ansible` directory. `cd ansible`


### Create and activate virtual env (optional)
```bash
python3 -m venv --clear ./venv
source ./venv/bin/activate
pip install -U pip setuptools wheel # Optionally
```

### Install ansible and tools
```bash
pip install -U ansible-core ansible ansible-lint ansible-navigator
```


### Install ansible collections and roles
```bash
./bin/install-ansible-roles
./bin/install-ansible-collections
```


### Run ansible playbooks
```bash
./bin/ansible-playbook init.yml
./bin/ansible-playbook node-exporter.yml
./bin/ansible-playbook docker.yml
```
