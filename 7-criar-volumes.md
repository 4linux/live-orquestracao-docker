# Criar volume mysql-data com plugin local-persist para o banco do Wordpress

sudo mkdir /mysql-data

docker volume create -d local-persist -o mountpoint=/mysql-data --name=mysql-data

# Criar volume wp-data com plugin nfs-volume-plugin para a app do Wordpress

docker volume create -d trajano/nfs-volume-plugin --opt device=seu-ip:/wpdata wp-data



