## Descripción

Can you find the flag on this website.

Additional details will be available after launching your challenge instance.
## Solución

picoCTF{G3tting_5QL_1nJ3c7I0N_l1k3_y0u_sh0ulD_98236ce6}
## Notas Adicionales

la pagina forma un login vulnerable Primero **bypasseas** la autenticación con una carga clásica como `' OR 1=1 --` para entrar. Después exploras la aplicación (hay un buscador/endpoint) y usas SQLi (p. ej. `UNION SELECT` o inputs que hacen match con una regex) para leer el contenido donde está la flag
Muestra por qué no confiar en la entrada del usuario
## Referencias
https://siunam321.github.io/ctf/picoCTF-2023/Web-Exploitation/More-SQLi

