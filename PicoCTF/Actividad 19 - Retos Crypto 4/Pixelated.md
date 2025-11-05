## Descripción

I have these 2 images, can you make a flag out of them? [scrambled1.png](https://mercury.picoctf.net/static/e8054e22552c6aba591cdf7440eb25e4/scrambled1.png) [scrambled2.png](https://mercury.picoctf.net/static/e8054e22552c6aba591cdf7440eb25e4/scrambled2.png)
## Solución

picoCTF{d72ea4af}
## Notas Adicionales

use este codigo de python y movi obiamente los 2 archivos a esa carptea y ya me imprime la bandera: 
from PIL import Image # pip install Pillow
img1 = Image.open("scrambled1.png")
pixels1 = img1.load()
img2 = Image.open("scrambled2.png")
pixels2 = img2.load()

flag = Image.new("RGB", img1.size)
flagpix = flag.load()

for row in range(img1.size[1]):
    for col in range(img1.size[0]):
        flagpix[col, row] = (
            (pixels1[col, row][0] + pixels2[col, row][0]) % 256,
            (pixels1[col, row][1] + pixels2[col, row][1]) % 256,
            (pixels1[col, row][2] + pixels2[col, row][2]) % 256
        )

flag.save("flag.png")
## Referencias

https://www.youtube.com/watch?v=e7Yx2nxGcqU
