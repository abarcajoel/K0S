 # Proceso para la instalación de K0S en dos Servidores
 1. # Generar claves con ssh para tener accesso a los servidores.
 ## ssh-keygen 
 # Copiar la clave a los dos servidores
 ## ssh-copy-ide nombreserver@ipserver

 # Instalación de K0s
 ## wget https://github.com/k0sproject/k0sctl/releases/download/v0.8.4/k0sctl-linux-x64


   # Movemos  a la carpeta correspondiente
 ## mv k0sctl-linux-x64

 # Damos Permisos
 ## chmod 777 k0sctl

 ## Comprobamos ./k0sctl
 ![img](https://github.com/abarcajoel/K0S/blob/main/img/instalacion.png)

 ## Como tenemos dos servidores crearemos el fichero de configuración  .yaml y en el indicaremos las ip's de cada servidor
 ## Creación del archivo yaml con init
 ## ./k0sctl init  Nos devuelve el archivo por defecto (realizar desde exterior).
 ![img](https://github.com/abarcajoel/K0S/blob/main/img/k0sctl_init.png)
 ## ./k0sctl init > k0sctl.yaml crearemos el nuevo archvivo pero con algunas mosdificaciones.
 ![img](https://github.com/abarcajoel/K0S/blob/main/img/archivo_yaml_dos_hosts.png)
