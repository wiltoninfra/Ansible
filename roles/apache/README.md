Role Name
=========

Servidor Apache 2.X.

Requirements
------------

Se você estiver usando SSL / TLS, você precisará fornecer seu próprio certificado e arquivos de chaves. Você pode gerar um certificado auto-assinado com um comando como openssl req -x509 -nodes -days 365 -newkey rsa:2048 -keyout example.key -out example.crt.

Role Variables
--------------

As variáveis ​​disponíveis estão listadas abaixo, juntamente com os valores padrão (veja defaults/main.yml):

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
