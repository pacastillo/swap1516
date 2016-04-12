# PRACTICA 3
# BALANCEO DE CARGA

**1. NGINX**

**1.1. Clave del repositorio.**

Lo primero que debemos realizar es importar la clave del repositorio software:

*cd /tmp/*

*wget http://nginx.org/keys/nginx_singing.key*

*apt-key add /tmp/nginx_singing.key/

*rm -f /tmp/nginx_singing.key*

![imagen](https://github.com/JaviMancilla/swap/blob/master/PRACTICAS/Practica_3/Capturas_nginx/1.PNG)

*NOTA: Para poder iniciar uno de los dos servicios, debemos parar/matar el otro servicio, ya que cada utiliza el puerto 80 y los dos a la vez no pueden usarlo.*
