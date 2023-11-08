# Ansible Dependency Chain

Repo for reproducing [Ansible bug #82154](https://github.com/ansible/ansible/issues/82154)

## Startup

- Initialize and activate virtualenv (using Python3.11)
  ```bash
  python3.11 -m virtualenv venv
  source ./venv/bin/activate
  ```
- Install Ansible
  ```bash
  pip install -r ./requirements.txt
  ```
- Install Ansible dependencies
  ```bash
  ansible-galaxy install -r ./requirements.yml
  ```
- Try to run a playbook
  ```bash
  ansible-playbook ./main.yml
  ```
