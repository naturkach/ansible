# ansible

hostfile:
<code>
[staging_servers]
linux1 ansible_host=<ip/hostname> ansible_user=ec2-user
</code>
cat ansible.cfg 
<code>
[defaults]
host_key_checking = false
inventory         = ./hosts.txt
  </code>
  
run only need task:
  - <b>ansible-playbook first.yml --tags "install_stress"</b>

