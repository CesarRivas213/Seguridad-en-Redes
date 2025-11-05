## Descripción

How about some hide and seek heh?Look at this image [here](https://artifacts.picoctf.net/c/237/atbash.jpg).
## Solución

picoCTF{atbash_crack_05b2a65a}
## Notas Adicionales

abrimos el archivo atbash como -> file atbash.jpg, con el comando ( steghide extract -sf atbash.jpg) que sirve para extraer datos ocultos dentro de un archivo, suelta un txt (encrypted.txt) y suelta un código, en cyberchef puedes transformarlo y sale la bandera
## Referencias

cyberchef  -> atbash