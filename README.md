## This is repository for launch EC2 using Ansbile Automation tool



##For secrets.yaml##    kindly use ansible_vault to create this (It is mentioned in playbook)
ansible-vault create secrets.yaml  ## Run this command and then it will ask for password you can set any password

Then store these values:-

key_name: put the name of ssh key name
security_group: put the secrity group name
vpc_subnet_id: put the vpc subnet id  

##Finally to run Ansible playbook
ansible-playbook -i inventory.ini ec2launch.yaml --ask-vault-pass  ###It will ask to enter password so enter the already defined password



Important Note:-I have already 1 EC2 already running on AWS where Ansbile is installed and boto, boto3 botocore and collection amazon.aws are installed . 


You have to also setup for AWS access key & AWS secret key on Ansible master node to access on AWS .

It can be done export as ENV.










