
curl -fsSL https://get.docker.com -o get-docker.sh && sudo sh get-docker.sh

sudo systemctl enable docker && sudo systemctl start docker


sudo usermod -aG docker seu-user


