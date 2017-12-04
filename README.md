Install and configuration Ansible
===========================

### Criar Chave de Acesso

ssh-keygen

ssh-copy-id -i  - para configurar a chave no servidor remoto

ssh -i  /etc/chave_acesso  usuario@maquina ‘comando a ser executado remoto’

Install version update
apt-add-repository ppa:ansible/ansible


Arquivo de configuração global - ansible.conf
Arquivo de inventario - hosts
Arquivos YAML regras - roles

Criar pasta chamada playbooks

Realizar configuração do arquivo ansible.conf

configurar linhas

:%d - apaga todo arquivo com vim

private_key_file
timeout
log_path
roles_path



comandos ansible

ansible all -m command -a "comando a ser executado"

