# ansible-playbooks
Common Ansible playbooks

## basic-env.yml
A playbook to setup basic environment. It would install python, docker, pip, awscli, etc.  
### How to use
```
ansible-playbook -u <remote-ssh-user> --key-file '<remote-ssh-keyfile>' -i '<remote-ip>,' \
    -e 'SSH_KEY="<ssh-key>"' basic-env.yml
```
### Example
```
ansible-playbook -u ubuntu --key-file '/home/david74/david74.pem' -i '13.115.245.247,' \
    -e 'SSH_KEY="ssh-rsa AABBCCDD david74"' basic-env.yml
```
