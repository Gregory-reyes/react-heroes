# se descargó la aplicación ejecutamos yarn install para instalar las dependencias
```	
yarn install
```
```
yarn build
```
# se ejecuta el comando yarn start  yarn dev para iniciar la aplicación
```
yarn dev 
yarn start
```
# descargamos la imagen de nginx version 1.23.3 con el siguiente comando
```
docker run --name some-nginx -d -p 8080:80 nginx:1.23.3
```
# entrar al contenedor de manera interactiva
```
docker exec -it 0fa bash
```
# copiamos el dockerfile de github actions creada

## ejecutanos el siguiente comando para crear la imagen y la miramos con ls
```
docker build -t heroes-app . --no-cache
```
# comando para correr la imagen
```
docker run -d -p 80:80 heroes-app
```
# entramos al modo interactivo del contenedor
```
docker exec -it 0fa bash
```
# ejecuto la ruta para copiar el archivo que voy a pegar en un archivo nginx.conf
```	
ruta: /etc/nginx/conf.d/default.conf
```
# con un cat entramos a default.conf y pegamos el archivo que copiamos

# creamos una carpeta nginx y archivo nginx.conf 




