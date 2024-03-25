# Ansible-PBXServer
Setup Playbooks For PBX Server.

If you haven't already for your user locally run: ssh-keygen -b 4048 -t rsa -C "root login" -N ""

That doesn't use a password

To persist it: ssh-copy-id root@pbx.local

Sometimes Root access is disabled.  If so:
echo 'PermitRootLogin=yes'  | sudo tee -a /etc/ssh/sshd_config
sudo systemctl restart sshd
