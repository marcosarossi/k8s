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
