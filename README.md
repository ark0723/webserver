# HTTPS Connection Test
- Using Docker on AWS EC2
- reference: https://github.com/wmnnd/nginx-certbot/tree/master
- Trouble Shooting
    - 1. SSH access: operaations time out 
    - cause: with HTTPS allowed setting, ufw enabled 
    - solution: stop EC2, edit USER DATA, paste "#!/bin/bash ufw diable iptables -L iptables -F --//"

