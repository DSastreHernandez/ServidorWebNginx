# Servidor Web Nginx
## Instalacion
Lo primero de todo es tener una distribucion linux/ubnuntu, yo en mi caso me he creado una maquina virtual con ubuntu, y hacemos un "apt-get update" y luego un "apt install nginx"
![Captura desde 2022-05-06 20-14-00](https://user-images.githubusercontent.com/91556389/167195209-327d32f5-fdba-4114-be7b-4c11824612ad.png)

Y ahora para comprobar que esta descargado, vamos al navegador y ponemos localhost y podremos ver que nginx nos da la bienvenida
![Captura desde 2022-05-06 20-22-35](https://user-images.githubusercontent.com/91556389/167196293-bd043b68-c404-4bb4-9f26-813224c96b68.png)

## Configuracion
Vamos a la carpeta /etc/nginx/ con el comando "cd" y en ella buscamos los archivos "sites-available" y "sites-enabled"

![Captura desde 2022-05-06 23-02-01](https://user-images.githubusercontent.com/91556389/167216066-819dffcd-8b09-44ad-8779-db95fb595bbe.png)

Ahora vamos a sites-available y con el comando cp hacemos una copia del documento default con el nombre que querrremos usa.

![Captura desde 2022-05-06 23-11-15](https://user-images.githubusercontent.com/91556389/167217169-e42600c3-9082-4956-a522-1196b17b774e.png)

Y ahora con un nano o un vim si lo tenemos instalado editamos los dos documentos que hemos copiado.
Y en los dos cambiamos esto respectivamente.

![Captura desde 2022-05-06 23-15-54](https://user-images.githubusercontent.com/91556389/167217648-8daeb075-e6be-4558-80b2-85f21e67bb2a.png)

![Captura desde 2022-05-06 23-35-30](https://user-images.githubusercontent.com/91556389/167219474-2dc351a0-0001-4a22-876c-7e29ca5bbe7e.png)

Ahora vamos a la carpeta /etc/nginx/sites-enabled/ y con el comando "ln -s" y la ruta de los archivos los linkamos aqui

![Captura desde 2022-05-06 23-44-53](https://user-images.githubusercontent.com/91556389/167220739-3ab57b62-6e82-4f2d-a65f-54e5fd146189.png)


