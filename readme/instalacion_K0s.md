 # Proceso para la instalación de K0S en dos Servidores
 1. Generar claves con ssh para tener accesso a los servidores.
 ## ssh-keygen 
 2. Copiar la clave a los dos servidores
 ## ssh-copy-ide nombreserver@ipserver

 3. Instalación de K0s
 ## wget https://github.com/k0sctl/releases/download/v0.8.4/k0sctl-linux-x64

   Movemos  a la carpeta correspondiente
 ## mv k0sctl-linux-x64

 Damos Permisos
 ## chmod 777 k0sctl