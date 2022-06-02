# Ejemplo Ansible

- Crear 4 VM de Linux
	- Una para Ansible
	- Una para MySQL
	- Una para Apache
	- Una para Docker 
- Verificar la IP de las VMs con `ip a`
- Loguearse por SSH a la VM que vaya a usar Ansible
- En esa VM ejecutar `yum install -y epel-release -y && yum install ansible -y` 
- Clonar el repo a la VM 
- Crear un inventario nuevo, tomando el de ejemplo como base, en un archivo llamado "inventario"
- Ejecutar: 
	- ansible-playbook -i inventario comun.yml 
	- ansible-playbook -i inventario apache-php.yml
	- ansible-playbook -i inventario mariadb.yml
	- ansible-playbook -i inventario docker 
