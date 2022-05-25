### Installation with Vagrant

💎 Vagrant templates and boilerplates for various projects 

Make sure you have [Vagrant](https://www.vagrantup.com/) and
[VirtualBox](https://www.virtualbox.org) installed.
In the root directory of the project, execute:

```
vagrant up
vagrant ssh
cd /vagrant
lein koan run
```


## Probable errors:

If windows user profile contains error msg: `incompatible character encodings: CP852 and Windows-1250`  
go to: `C:\HashiCorp\Vagrant\embedded\gems\2.2.19\gems\vagrant-2.2.19\bin\vagrant`

```
#!/usr/bin/env ruby

Encoding.default_external = Encoding.find('Windows-1250')
Encoding.default_internal = Encoding.find('Windows-1250')
```
&  

change Oracle VirtualBox VM location  & adding windows Enviroment Variable VAGRANT_HOME = C:\HashiCorp\Vagrant\.vagrant.d

> Enable-WindowsOptionalFeature -FeatureName ServicesForNFS-ClientOnly, ClientForNFS-Infrastructure -Online -NoRestar
