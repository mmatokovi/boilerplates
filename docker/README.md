### Installation with Vagrant

🛳️ Docker templates and boilerplates for various projects 

Make sure you have [Vagrant](https://www.vagrantup.com/) and
[VirtualBox](https://www.virtualbox.org) installed.
In the root directory of the project, execute:

```
vagrant up
vagrant ssh
cd /vagrant
```

## MySQL

add docker image `docker pull mysql` run container `docker run --name mysql -e MYSQL_ROOT_PASSWORD=secret -d mysql:latest` open *mysql* `mysql -uroot -p`