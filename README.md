first step
 ansible-playbook -i inventory.ini ec2_create.yaml

second step (inventory)
[webservers]
<EC2_PUBLIC_IP> ansible_user=ubuntu ansible_ssh_private_key_file=~/.ssh/mykey.pem

third step
ansible-playbook -i inventory.ini setup_webserver.yaml
