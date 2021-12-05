 # Proceso para la instalación de K0S en dos Servidores
 # 1.  Generar claves con ssh para tener accesso a los servidores.
 ## ssh-keygen 
 # 2. Copiar la clave a los dos servidores
 ## ssh-copy-ide nombreserver@ipserver

 # 3. Instalación de K0s
 ## wget https://github.com/k0sproject/k0sctl/releases/download/v0.8.4/k0sctl-linux-x64


# 4. Movemos  a la carpeta correspondiente
 ## mv k0sctl-linux-x64

 # 5. Damos Permisos
 ## chmod 777 k0sctl

 ## 6. Comprobamos ./k0sctl
 ![img](https://github.com/abarcajoel/K0S/blob/main/img/instalacion.png)

 ## Como tenemos dos servidores crearemos el fichero de configuración  .yaml y en el indicaremos las ip's de cada servidor
 # 7. Creación del archivo yaml con init
 ## ./k0sctl init  Nos devuelve el archivo por defecto (realizar desde exterior).
 ![img](https://github.com/abarcajoel/K0S/blob/main/img/k0sctl_init.png)
 ## ./k0sctl init > k0sctl.yaml crearemos el nuevo archvivo pero con algunas mosdificaciones.
 ![img](https://github.com/abarcajoel/K0S/blob/main/img/archivo_yaml_dos_hosts.png)
