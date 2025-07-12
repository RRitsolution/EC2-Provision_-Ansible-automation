##For secrets.yaml##    kindly use ansible_vault
ansible-vault encrypt secrets.yaml  ## Run this command and then it will ask for password you can set any password

Then store these values:-

key_name: put the name of ssh key name
security_group: put the secrity group name
vpc_subnet_id: put the vpc subnet id  

##Finally to run ANsbile playbook
ansible-playbook -i inventory.ini ec2launch.yaml --ask-vault-pass  ###It will ask to enter password so enter the already defined password






