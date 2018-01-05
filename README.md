Configuração de Ambiente Cloud - TBF HOST
===========================

### Criar Chave de Acesso

ssh-keygen

ssh-copy-id -i  - para configurar a chave no servidor remoto

ssh -i  /etc/chave_acesso  usuario@maquina ‘comando a ser executado remoto’

Instale a ultima versão do Ansible.

Realizar configuração do arquivo ansible.conf

configurar linhas

:%d - apaga todo arquivo com vim

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

```
ansible all -m command -a 'ls -la'
ansible-playbook -- syntax-check nome.yaml
// Using variable external
ansible-playbook -e username=developer users.yaml
//Padronizando usuários no linux com Ansible
```
Roles
==========

 ansible galaxy
Gerencia de Tecnologias
Dentro das roles existem arquivos main.yaml onde são definidas as regras
