This repo was created when I was practising Ansible

# Valut commands
1. openssl rand -base64 32 > .vault_pass.txt -> To create password
2. ansible-vault  -> to get options 
3. ansible-vault encrypt inventory.yml --vault-password-file .valut_pass.txt
4. ansible-vault encrypt inventory.ini --ask-vault-pass -> ask password
5. ansible-vault decrypt inventory.ini --vault-password-file .vault_pass.txt
6.  ansible-vault edit inventory.ini --vault-password-file .vault_pass.txt
7.  ansible-vault view inventory.ini --vault-password-file .vault_pass.txt

# Roles
to create a role 
1. ansible-galaxy role init httpd
2. ansible-galaxy import iamtruptimane devops-18-may-ansible-role --token <token>
3. ansible-galaxy role install iamtruptimane.devops-18-may-ansible-role