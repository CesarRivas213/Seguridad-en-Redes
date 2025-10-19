## Descripción

Decode this [message](https://jupiter.challenges.picoctf.org/static/14393e18d98fedbaedbc28896d7ef31a/message.wav) from the moon.
## Solución

picoCTF{beep_boop_im_in_space}
## Notas Adicionales

solo conviertes el audio en como si fuera una transmision de imagen lenta, instala qsstv y pavucontrol , ejecutas los 2 solo escribiendo su nombre , y luego este comando para establecer una conexion virtual entre el qsstv y pavucontrol($ pactl load-module module-null-sink sink_name=virtual-cable) y $ paplay -d virtual-cable message.wav

## Referencias
https://medium.com/@sobatistacyber/picoctf-writeup-m00nwalk-15a64699ac21

