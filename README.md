readme de la practica 2

Creamos un archivo vagrant file escribiendo: vagrant init -m

Empezamos a configurarlo añadiendo los sistemas operativos que quermaos poner, en mi ocasión Debian/bookworm64.
Al iniciar las máquinas virtuales (que tendrás que escribir vagrant up) probaremos a entrar en cada una para cer si funcionan, usando vagrant ssh "el_nombre_de _la_máquina", cuando entremos en el del servidor, escribiremos nano /etc/dhcp/dhcpd.conf para configurar el DHCP del servidor.
Cuando hemos terminado de configurar el DHCP, vamos a configurar la tarjeta de red para e servidor, en esta ocasión ponemos el comando /etc/default/isc-dhcp-server , y en el apratado de protocolo ipv4 ponemos la arjeta de red que tenga la ip que queramos poner como ip del servidor.
copiamos cada archivo a nuestro ordenador escribiendo cp /etc/dhcp/dhcpd.conf /vagrant y cp /etc/default/isc-dhcp-server /vagrant. Con esto conseguimos sacar los archivos para tenerlos como platnillas.
