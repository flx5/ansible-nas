# Using the Vault

Create secret:
```shell
ansible-vault encrypt_string --vault-password-file 'secret.txt' --name 'the_secret' string_to_encrypt
```

Run Playbook:
```shell
ansible-playbook --vault-password-file secret.txt playbooks/site.yml 
```