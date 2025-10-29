# Devops.Works helm charts

This repository hosts [Devops.Works](http://devops.works/) helm charts.

## Authors

[@devops-works](https://github.com/devops-works)

# Documentacion despliegue Cyberchef
Felipe Velasco
## Pasos para desplegar    

1. Ya esta creado el helm y sus templates
    ```bash 
    ##helm create cyberchef
    ```
2. Probamos el deplyment
 ```bash 
helm install --debug --dry-run workshop <ruta de la carpeta creada en el paso anterior>
```
![Prueba](/helm-charts/cyberchef/foto3.png)

3. Y desplegamos
```bash 
helm install cyberchef <pathtotemplate>
# Y corremos los comandos que dice la nota despues de instalarlo
# export POD_NAME...
# export CONTAINER_PORT...
#kubectl ... port forward...
kubectl get svc,po,deploy
```

4. Verificamos en la url y los servicios
```bash
kubectl get svc,po,deploy
```

![Plataforma desplegada](/helm-charts/cyberchef/foto1.png)
![Plataforma desplegada](/helm-charts/cyberchef/foto2.png)

