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
-------------
```
// Install Package
ansible all -m command -a "comando a ser executado"

// Fatos Informações que recupero de uma maquina, inventario.
ansible all -m setup

// Instalar pacote
ansible all -m package -a "name=vim state=present"

```
Links para Validador de YAML
http://www.yamllint.com/

Playbooks
==============

São Arquivos do ansible que descrevem as tarefas a serem executadas no servidor.
Padrão de identação
getent - Comando Linux
Projeto AWX
ansible all -m command -a 'cat /etc/resolv.conf'
ansible-playbook -- syntax-check nome.yaml
Using variable external
ansible-playbook -e username=developer users.yaml
Padronizando usuários no linux com Ansible

Roles
==========

 ansible galaxy
Gerencia de Tecnologias
Dentro das roles existem arquivos main.yaml onde são definidas as regras
