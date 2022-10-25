# Plugin de disco local

curl -fsSL https://raw.githubusercontent.com/MatchbookLab/local-persist/master/scripts/install.sh | sudo bash

sudo systemctl daemon-reload

sudo systemctl enable docker-volume-local-persist

# Plugin NFS

docker plugin install --grant-all-permissions trajano/nfs-volume-plugin

