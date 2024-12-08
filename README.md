#How to deploy nexus to target machine ?
1) ssh to target host create user alice
2) on /home/alice/.ssh/authorized_keys -----> add public key
3) Add alice to sudoers file
   alice   ALL=(ALL:ALL) NOPASSWD:ALL
5) clone repo
6) Go to Day3
7) update hosts file below [nexus] group add ip of machine you want to deploy nexus on
8) on root Direcory on Day3 run main playbook using
   ansible-playbook -i hosts --private-key /path/to/private/key main.yml
   
