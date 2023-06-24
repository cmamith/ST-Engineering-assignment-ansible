Modify the variables node_exporter_version, username, and password in the playbook according to your requirements.
Create an inventory file (e.g., inventory.ini) specifying the target Ubuntu virtual machines under the ubuntu_vms group.
Execute the playbook using the ansible-playbook command, providing the inventory file and playbook name

Make sure to replace your_username and your_repository with your actual  username and password

ansible-playbook -i inventory.ini install_node_exporter.yml --ask-vault-pass

I have used the ansible vault syntax just to make it more secure


Once the playbook is executed, it will install Prometheus Node Exporter on the specified Ubuntu virtual machines using the provided version and the specified username/password for connection.

