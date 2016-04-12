# PRACTICA 3
# BALANCEO DE CARGA

**1. NGINX**

  **1.1. Clave del repositorio.**

	Lo primero que debemos realizar será importar la clave del repositorio software:

	*cd /tmp/*
	*wget http://nginx.org/keys/nginx_singing.key*
	*apt-key add /tmp/nginx_singing.key/
	*rm -f /tmp/nginx_singing.key*

	A continuación añadimos el repositorio al fichero:

	*echo "deb http://nginx.org/packages/ubuntu/ lucid nginx" >> /etc/apt/sources.list*
	*echo "deb-src http://nginx.org/packages/ubuntu/ lucid nginx" >> /etc/apt/sources.list*


	![imagen](https://github.com/JaviMancilla/swap/blob/master/PRACTICAS/Practica_3/Capturas_nginx/1.PNG)



  **1.2. Instalación.**

	En este punto, una vez importada la clave del repositorio, instalamos el paquete "Nginx":

	*apt-get update*
	*apt-get install nginx*

	![imagen](https://github.com/JaviMancilla/swap/blob/master/PRACTICAS/Practica_3/Capturas_nginx/2.PNG)

  **1.3. Configuración del archivo default.conf.**

	![imagen](https://github.com/JaviMancilla/swap/blob/master/PRACTICAS/Practica_3/Capturas_nginx/3.PNG)


  **1.4. Comprobación.**


	![imagen](https://github.com/JaviMancilla/swap/blob/master/PRACTICAS/Practica_3/Capturas_nginx/6.PNG)

	![imagen](https://github.com/JaviMancilla/swap/blob/master/PRACTICAS/Practica_3/Capturas_nginx/7.PNG)





**2. HAPROXY**

  **2.1. Instalación.**

	Para la instalación de Haproxy solo debemos usar el siguiente comando:

	*apt-get install haproxy*

  **2.2. Configuración archivo.**

	*cd /etc/*
	*cd haproxy/*
	*nano haproxy.cfg*
	
	
	![imagen](https://github.com/JaviMancilla/swap/blob/master/PRACTICAS/Practica_3/Capturas_nginx/5.PNG)

  **2.3 Comprobación.**  

	![imagen](https://github.com/JaviMancilla/swap/blob/master/PRACTICAS/Practica_3/Capturas_nginx/6.PNG)

	![imagen](https://github.com/JaviMancilla/swap/blob/master/PRACTICAS/Practica_3/Capturas_nginx/7.PNG)   
  

  *NOTA: Para poder iniciar uno de los dos servicios, debemos parar/matar el otro servicio, ya que cada utiliza el puerto 80 y los dos a la vez no pueden usarlo.*

  