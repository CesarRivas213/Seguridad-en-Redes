## Descripción

Can you abuse the banner?The server has been leaking some crucial information on `tethys.picoctf.net 59764`. Use the leaked information to get to the server.To connect to the running application use `nc tethys.picoctf.net 63615`. From the above information abuse the machine and find the flag in the /root directory.
## Solución

picoCTF{b4nn3r_gr4bb1n9_su((3sfu11y_68ca8b23}
## Notas Adicionales

se crea un enlace simbolico /home/player/banner que apunta a /root/flag.txt . Y pues lee /root/flag.txt  
## Referencias
https://www.youtube.com/watch?v=M6N0IBIDp-Q
