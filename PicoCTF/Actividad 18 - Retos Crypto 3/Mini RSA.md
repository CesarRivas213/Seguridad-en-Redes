## Descripción

What happens if you have a small exponent? There is a twist though, we padded the plaintext so that (M ** e) is just barely larger than N. Let's decrypt this: [ciphertext](https://mercury.picoctf.net/static/2d884b04dbb44896dda1276774b09216/ciphertext)
## Solución
picoCTF{e_sh0u1d_b3_lArg3r_a166c1e3}

## Notas Adicionales
- Del _primer_ programa (ataque **small-e**) ejecuté la misma comprobación: calcular la raíz cúbica entera de `c` y ver si es exacta.
    
- Del _segundo_ programa (ataque **k-iterativa**) ejecuté la búsqueda de `k = 1..10000` y para cada `k` calculé `target = c + k*n` y comprobé si `target` es un cubo perfecto.

remplaze los datos de ciphertext 

Probé primero el ataque small-e (falló), luego el k-iterativo y **encontré k = 3533** que da la flag 
## Referencias
chat