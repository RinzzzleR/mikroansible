
# Список протестированного оборудования

# Microtic: Routerboard 2011 UIAS-IN
# SwOS: L5


Установка Ansible проста, так как все из коробки:

sudo apt-add-repository ppa:ansible/ansible
sudo apt-get update
sudo apt-get install ansible


Создать в системе не привилегированного пользователя, например, mikroansible 
` adduser mikroansible`

Стать этим пользователем 
`su - mikroansible`

Создать пару RSA ключей
`ssh-keygen`

Установить pwgen 
`apt-get install pwgen` 

Настроить параметры SSH клиента файл ~/.ssh/config
   
    Host * 
    ServerAliveInterval 4
    ServerAliveCountMax 5
    ConnectTimeout 10
    NumberOfPasswordPrompts 0
    StrictHostKeyChecking yes
