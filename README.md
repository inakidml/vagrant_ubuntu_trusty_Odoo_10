# vagrant_ubuntu_trusty_Odoo_10
vagrantfile para maquina virtual ubuntu conodoo instalado

### Clonaar repositorio
```bash
git clone https://github.com/inakidml/vagrant_ubuntu_trusty_Odoo_10
```
```bash
cd vagrant_ubuntu_trusty_Odoo_10
```
### Arrancar maquina
```bash
vagrant up
```
## Datos de Acceso
Esta mapeado el puerto 8069 del Localhost al 8069 de la maquina, asi que podemos conectarnos a Odoo desde cualquier navegador escribiendo:

http://localhost:8069

Podemos añadirle una ip pública para poder acceder desde cualquier pc de la red, descomentando en el Vagrantfile la linea:
>config.vm.network "public_network", ip: "192.168.1.4"     .
y poniendo una ip de nuestro rango.


