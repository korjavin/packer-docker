Build docker image provisioned from puupet master by packer.io

packer build -var 'puppet_master=fqdn.my.puppet.master' docker.json




On puppet master machine you should set autosign

Like *.mydomain in autosign.conf

And if you are using puppet fileserver, then add
[files]
  ...
  allow *.mydomain


into fileserver.conf
