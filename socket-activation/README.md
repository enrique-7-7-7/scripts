sudo systemctl stop ssh.service
sudo systemctl disable ssh.service

sudo systemctl enable ssh.socket
sudo systemctl start ssh.socket

sudo systemctl status ssh.socket

sudo ufw allow ssh



systemctl status ssh.service
systemctl status ssh.socket


sudo systemctl stop ssh.socket
sudo systemctl disable ssh.socket
sudo systemctl enable --now ssh.service


sudo systemctl stop ssh.service
sudo systemctl disable ssh.service
sudo systemctl enable --now ssh.socket

