First you need to take a Clone of a Repository.

You need to checkout Main Branch.

There is a main file called deploy_docker.yml file.

If you want to add a custom change that should rendor when you hit the host or target machine ip on the browser.Then you need to change the path(cp <path/to your/index.html file> apache_container:/usr/local/apache2/htdocs/)

inventory.ini consist of host ip and the user through which we can ssh from local to target machine.

command to run playbook :- ansible-playbook -i inventory.ini deploy_docker.yml

The host machine ip needs to be change and user need to be changed that can ssh.
