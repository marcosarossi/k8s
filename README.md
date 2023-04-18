# Comandos útiles

# minikube
Todos los comandos se usan con permisos de administrador/root
## Iniciar cluster
```console
minikube start
```
## Detener cluster
```console
minikube stop
```

## Obtener url para acceder a servicio desde el host
```console
minikube service <service-name> --url
```

## Acceder al dashboard
```console
minikube dashboard
```

## Habilitar el addon ingress
```console
minikube addons enable ingress
```

## Montar directorio local en VM de minikube
```console
minikube mount <source directory>:<target directory>
```

# docker

## Usar el registry de dockers local

```console
minikube docker-env | Invoke-Expression # Usando powershell

cd ./jsat
docker build -t telpin-jsat-main images/jsat-main
docker build -t telpin-jsat-ov images/jsat-ov
#docker run -d --name jsat1 telpin-jsat-main
```

# kubernetes
## Recuperar los namespaces disponibles
```console
kubectl get namespaces
kubectl get ns
```

## Recuperar los namespaces disponibles
```console
kubectl get all
```

## Aplicar un .YML
```console
kubectl apply -f pv-postgres.yml
```

## Correr comandos dentro de un POD
```console
kubectl exec -it pod-tomcat -- sh
```
## Herramienta para monitorear red (creando contenedor efímero)
```console
kubectl debug POD_NAME -it --image=nicolaka/netshoot
```

## Ingress
```console
kubectl get ingress
```