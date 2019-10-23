# Ansible role for Java development environment

Install:

    $ ansible-galaxy install chrgue.java_development


Playbook example:

    - name: Setup java development enviroment
      hosts: all
      connection: local
      roles:
        - role: chr.java_development
          become: yes
        

Ad-Hoc:

    $ sudo apt install wget
    $ bash <(wget -qO- https://raw.githubusercontent.com/chrgue/ansible-role-java/master/adhoc.sh)