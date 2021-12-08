# Vamos a comprobar el funcionamiento de nuestro servidor 
## 1. Crearemos un pod en este caso con replicaset para tener dos
![img](https://github.com/abarcajoel/K0S/blob/main/img/pod_joel.png)
## 2. Lo lanzaremos con k0s kubectl apply -f nombre-archivo.yaml en este caso con nginx
![img](https://github.com/abarcajoel/K0S/blob/main/img/replicaset_nginx.png)
## Vemos que se haya creado junto con las replicas
![img]()
## 3. Entramos en nuestro pod y modificamos el html por defecto y añadimos algo nuevo
![img]()
## 4. Creamos pasarela con k0s kubectl port-forward nombre-pod puertoexterior:puertointerior
![img]()
## 5. Comprobamos con el comando curl localhost:puertoexterior
![img]()