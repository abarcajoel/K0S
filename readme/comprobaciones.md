# Vamos a comprobar el funcionamiento de nuestro servidor 
## 1. Crearemos un pod 
## 2. Lo lanzaremos con ./k0sctl kubectl apply -f nombre-archivo.yaml
## 3. Entramos en nuestro pod y modificamos el html por defecto y añadimos algo nuevo
## 4. Creamos pasarela con ./k0sctl kubectl port-forward nombre-pod puertoexterior:puertointerior
## 5. Comprobamos con el comando curl localhost:puertoexterior