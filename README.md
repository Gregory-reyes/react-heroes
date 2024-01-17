## se descargó la aplicación ejecutamos yarn install para instalar las dependencias
```	
yarn install
```
```
yarn build
```
## se ejecuta el comando yarn start  yarn dev para iniciar la aplicación
```
yarn dev 
yarn start
```
## descargamos la imagen de nginx version 1.23.3 para copiar información de nginx para nuestra carpeta de build despues se puede eliminar la imagen nginx:1.23.3

```
docker run --name nombre -d -p 8080:80 nginx:1.23.3
```
## entrar al contenedor de manera interactiva
```
docker exec -it 0fa bash
```
## ingresamos a la ruta descrita copiamos el archivo default.conf con un cat lo copiamos para pegarlo en nuestro nuevo archivo nginx.conf
```
cd etc/nginx/conf.d
```
## copiamos todo lo de default en una nueva carpeta nginx y un archivo nginx.conf y pegamos todo lo que esta entre llaves de server

## copio la siguiente linea de comando en location debajo del index.htm del archivo creado nginx.conf
```
try_files $uri $uri/ /index.html;
```

## Construimos la nueva imagen con el siguiente comando 
```
docker build -t heroes-app . --no-cache
```
## comando para correr la imagen
```
docker run --name nombre -d -p 80:80 heroes-app
```









