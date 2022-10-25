# Criando Disco

Discos > defina o nome do disco > defina o tamanho de 10 GB > salvar



# Anexando novo Disco

Vá em editar VM > Discos Adicionais > selecione o disco  e aperte em salvar > Por fim salve as edições na VM


# Dentro da VM


2 - Acessar a instância
3 - Usar o comando sudo fdisk -l para identificar o disco
4 - Aplicar o sistema de arquivos no disco: sudo mkfs.xfs /dev/sdb
5 - Criar o ponto de montagem: sudo mkdir /mysql-data
6 - Realizar a montagem: sudo mount -t xfs /dev/sdb /mysql-data
7 - Configurar a montagem automática no arquivo /etc/fstab: /dev/sdb /mysql-data xfs defaults 0 0