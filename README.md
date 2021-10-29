## Install Ansible on Client
```bash
sudo apt-get update
sudo apt-get install -y python3-pip
pip3 install ansible
which ansible-playbook
```

## If the command is not found after install, add the Python modules to PATH
```bash
echo 'export PATH="$HOME/.local/bin:$PATH"' >> $HOME/.bash_profile
```

## Run Playbook from Client
```bash
ansible-playbook -i inventory.yml ./playbook.yml
```

### Optional playbook parameters
```bash
--ask-pass --ask-become-pass
```
```bash
--vault-password-file ./vault_password_file
```
```bash
--ask-vault-password
```