## Descripción
In RSA, a small `e` value can be problematic, but what about `N`? Can you decrypt this? [values](https://mercury.picoctf.net/static/2604f8b51a5cc62d38a3736938f19cef/values)

## Solución

picoCTF{sma11_N_n0_g0od_13686679}
## Notas Adicionales

si `n` es factorizable (o está en FactorDB), obtienes `p` y `q`. Con `p,q` puedes calcular φ(n) y la clave privada `d`, y descifrar `m = c^d mod n`

- Buscar si `n` ya está en **FactorDB** (rápido) o intentar factorizarlo con herramientas automáticas (RsaCtfTool) o Pollard-Brent/Pollard-Rho.
    
- Si obtienes `p` y `q` entonces:
    
    - `phi = (p-1)*(q-1)`
        
    - `d = inverse(e, phi)` (modular inverse)
        
    - `m = pow(c, d, n)`
        
    - convertir `m` a bytes: `hex(m)` → ajustar longitud par → `bytes.fromhex(...)` → `decode('utf-8')`
        
- La salida decodificada suele contener la flag en formato `picoCTF{...}`; quitar cualquier padding alrededor.


python3 RsaCtfTool.py -n <n> -e 65537 --uncipher <c>

##REFERENCIAS

https://factordb.com
chat
RsaCtfTool

