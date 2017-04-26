# Vagrant Ubuntu trusty Odoo 10
######Vagrantfile para maquina virtual ubuntu 16.04 con Odoo 10.0 instalado

#####Es necesario tener [VirtualBox](https://www.virtualbox.org/wiki/Downloads), [Vagrant](https://www.vagrantup.com/downloads.html) y [Git](https://git-scm.com/downloads) instalado.

### Clonar repositorio
```bash
git clone https://github.com/inakidml/vagrant_ubuntu_trusty_Odoo_10
```
```bash
cd vagrant_ubuntu_trusty_Odoo_10
```
### Arrancar máquina
```bash
vagrant up
```
## Datos de Acceso
Esta mapeado el puerto 8069 del Localhost al 8069 de la máquina, asi que podemos conectarnos a Odoo desde cualquier navegador escribiendo:

[http://localhost:8069](http://localhost:8069)

*Correo electronico: 
admin@odoo.es*

*Contraseña: 
admin*

Podemos añadirle una ip pública para poder acceder desde cualquier pc de la red descomentando en el Vagrantfile la línea:
>config.vm.network "public_network", ip: "192.168.1.4"

y poniendo una ip de nuestro rango.

### Apagar máquina
```bash
vagrant halt
```
### Conectarnos por ssh
```bash
vagrant ssh
```
### Eliminar máquina
```bash
vagrant destroy
```

### Reiniciar servidor Odoo
```
sudo service odoo restart
```



### Ruta modulos 
```bash
/usr/lib/python2.7/dist-packages/odoo/addons/
```

