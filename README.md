# ansible
ansible playbooks used
    ## nginx key add ##
    ansible webdb -b -K  -m shell -a "cd /tmp && wget http://nginx.org/keys/nginx_signing.key; cd /tmp &&  apt-key add     nginx_signing.key;" -u ctuser -f 30

    ansible-playbook work.yml -u ctuser --ask-become-pass -f 40
