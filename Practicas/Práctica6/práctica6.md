** Practica 6: Discos en RAID **
=======================================================


Empezamos creando 2 discos duros virtuales en la máquina virtual, del mismo tipo que el que tiene instalado el sistema operativo.

Instalamos la aplicación mdadm.

sudo apt-get install mdadm y vemos que la identificacion asignada por ubuntu a los discos es sdb y sdc

Ahora creamos el nivel RAID 1

<img src="./img/img1.png"/>

Le damos formato  al dispositivo RAID

<img src="./img/img2.png"/>

Creamos la carpeta /dat y la montamos en el dispositivo RAID

<img src="./img/img3.png"/>

<img src="./img/img4.png"/>

Comprobamos el estado de RAID, en este caso lo hacemos con md127 porque ya hemos reiniciado.

<img src="./img/img5.png"/>

Ahora comprobamos el uuid del dispositivo con ls -l /dev/disk/by-uuid/

<img src="./img/img6.png"/>

Y editamos el fichero /etc/fstab añadiendo la siguiente linea

<img src="./img/fstab.png"/>

Ahora simulamos un fallo en uno de los discos en este caso el sdc

<img src="./img/img7.png"/>

Miramos los detalles

<img src="./img/img8.png"/>

Borramos el disco.

<img src="./img/img9.png"/>

Vemos en los detalles que está eliminado.

<img src="./img/img10.png"/>

Ahora añadimos el disco de nuevo y vemos como se vuelve a sincronizar

<img src="./img/img11.png"/>

<img src="./img/img12.png"/>


















