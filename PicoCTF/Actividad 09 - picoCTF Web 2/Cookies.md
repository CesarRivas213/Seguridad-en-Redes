## Descripción

Who doesn't love cookies? Try to figure out the best one. [http://mercury.picoctf.net:27177/](http://mercury.picoctf.net:27177/)
## Solución


picoCTF{3v3ry1_l0v3s_c00k135_064663be}


## Notas Adicionales

Solo es enviar distintas solicitudes , lo automatizas para no tardar tanto
for i in {0..20}; do curl -s http://mercury.picoctf.net:6418/check -H "Cookie: name=$i"; done | grep picoCTF
## Referencias
kali linux