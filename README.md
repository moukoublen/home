# Home infrastructure
Home infrastructure scripts

## Ansible

Everything of the above needs to be run inside `ansible` directory. `cd ansible`


### Create and activate virtual env (optional)
```bash
python3 -m venv --clear ~/python-env
source ~/python-env/bin/activate
pip install -U pip setuptools wheel # Optionally
pip install -U ansible-core ansible ansible-lint ansible-navigator
```


### Install ansible collections and roles
```bash
./bin/install-ansible-lib
```
