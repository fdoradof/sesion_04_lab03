# sesion_04_lab03
Laboratorio de facts

# Enunciado del Ejercicio

* Nota: Antes de empezar la practica debemos de añadir a través de Hyper-V un disco de 2Gb al nodo_01

- Crearemos u repositorio en GitHub con el nombre sesion_04_lab03
- Lo clonaremos en nuestro equipos
- Insertaremos el inventario y el ansible.cfg necesario para conectarnos a los nodos
- Creamos un playbook con el nombre "playbook.yml"
- Titularemos el playbook "Laboratorio de Facts"
- Haremos un play que ataque al nodo_01, el cual realizara las siguientes tareas:
	- Listara todos los facts del nodo
	- Crearemos un archivo llamado datos_NOMBRE_NODO (variables)
	- Con ayuda de los facts insertaremos los siguientes datos:
		- Lista de los dispositivos de red indicando los siguientes datos de cada uno de ellos:
			- IP
			- MACADDRES
			- GATEWAY
			- NETMASK
		
		- Lista de dispositivos de almacenamiento con la capacidad total de cada uno de ellos
	- Configuraremos el disco que añadimos antes de empezar la practica, este debe tener:
		- partición
		- pv
		- vg llamado vg_prueba
		- lv llamado lv_prueba
		- fs con estension xfs
		- Montarlo en /mnt/prueba
	
	- Actualizaremos la lista de facts con los nuevos datos del nuevo disco
