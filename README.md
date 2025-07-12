##For secrets.yaml##    kindly use ansible_vault
ansible-vault encrypt secrets.yaml  ## Run this command and then it will ask for password you can set any password

##Finally to run ANsbile playbook
ansible-playbook -i inventory.ini ec2launch.yaml --ask-vault-pass  ###It will ask to enter password so enter the already defined password






