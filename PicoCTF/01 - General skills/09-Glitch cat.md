
## Descripción 

Our flag printing service has started glitching!

Additional details will be available after launching your challenge instance.

## Solución

picoCTF{gl17ch_m3_n07_a4392d2e}
## Notas Adicionales

Se puede hacer en python importando socket
`import socket

HOST = 'jupiter.challenges.picoctf.org'
PORT = 7480

with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
    s.connect((HOST, PORT))
    data = s.recv(4096)
    print(data.decode('utf-8'))`
## Referencias
python