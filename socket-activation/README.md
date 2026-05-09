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

---

sudo nano /lib/systemd/system/ssh.socket
mkdir -p /etc/systemd/system/ssh.socket.d
cat >/etc/systemd/system/ssh.socket.d/listen.conf <<EOF [Socket] ListenStream= ListenStream=1234 EOF


---
<img width="660" height="199" alt="Screenshot from 2026-05-09 12-12-19" src="https://github.com/user-attachments/assets/f40c51f4-da2a-43bf-b0f3-db8c13b3f391" />
