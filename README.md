# CNC-Impresion-Laser
Conjunto de Software necesarios para hacer funcionar la impresora láser. Antes de empezar, es necesario descargar e instalar 3 cosas (elige tu sistema operativo):

## WINDOWS
```
1º Drivers de la impresora: https://sparks.gogo.co.nz/assets/_site_/downloads/CH34x_Install_Windows_v3_4.zip
2º Ilustrador: https://inkscape.org/gallery/item/33464/inkscape-1.2_2022-05-15_dc2aedaf03-x64_FKau6eX.exe
3º Laminador: https://github.com/LightBurnSoftware/deployment/releases/download/1.1.04/LightBurn-v1.1.04.exe
```

## LINUX
```
1º Drivers de la impresora: https://sparks.gogo.co.nz/assets/_site_/downloads/CH340_LINUX.zip
2º Ilustrador: https://inkscape.org/gallery/item/33450/Inkscape-dc2aeda-x86_64.AppImage
3º Laminador: https://github.com/LightBurnSoftware/deployment/releases/download/1.1.04/LightBurn-Linux64-v1.1.04.run
```

## MAC
```
1º Drivers de la impresora: https://github.com/adrianmihalko/ch340g-ch34g-ch34x-mac-os-x-driver/raw/master/CH34x_Install_V1.5.pkg
2º Ilustrador: https://inkscape.org/gallery/item/33440/Inkscape-1.2.0_x86_64.dmg
3º Laminador: https://github.com/LightBurnSoftware/deployment/releases/download/1.1.04/LightBurn.V1.1.04.dmg
```

# Procedimiento
Si ya has instalado todo lo mencionado justo antes, podemos pasar al procedimiento. A continuación, te diré cómo deberás usar las herramientas para hacer funcionar la CNC correctamente.

> **1º paso:** Elige tu imagen, y adjuntala en un nuevo proyecto de **InkScape** (uno de los programas que te has descargado antes)

<img width="1912" alt="acb" src="https://user-images.githubusercontent.com/75345847/172207011-f05b9324-d742-4461-b1ac-6e5504daa525.png">

> **2º paso:** Accede a la ventana de **Trayecto** y selecciona la opcion **Vectorizar mapa de bits**. A la derecha aparecera un menu con diferentes opciones. Simplemente, seleccione la ventana que pone **Varias pasadas** y establece la misma configuracion que aparece en una de las siguientes imagenes. Cuando domines mejor el programa, podrás experimentar con parámetros distintos. Una vez hecho, dale a **Aplicar**.

<img width="1918" alt="acb" src="https://user-images.githubusercontent.com/75345847/172207212-5a852397-cddd-41dd-aadb-debf73727048.png">
<img width="816" alt="acb" src="https://user-images.githubusercontent.com/75345847/172207432-8f03136f-003b-4858-b94a-efef484c9d55.png">

> **3º paso:** Si haces click sobre la imagen y la arrastras, veras que se ha generado una o mas versiones de la imagen, pero con distintos tonos y rasgos. Quédate con aquella que mayor contraste tenga (donde se distinga mejor los blancos de los negros) y borra todas las demás. La imagen sobre la que trabajarás, será esa.

<img width="1915" alt="acb" src="https://user-images.githubusercontent.com/75345847/172208165-412dd1e9-31a2-43e2-b7ea-abcd0669b668.png">
<img width="1916" alt="acb" src="https://user-images.githubusercontent.com/75345847/172208286-b5be16af-a96c-4c54-bab8-21d1f1d9b4a0.png">

> **4º paso:** Accede a la ventana **Objeto** y haz click sobre la opcion **Relleno y borde**. Asegurate de tener seleccionada la imagen, y estando seleccionada, aparecerá un menu a tu derecha, en donde apareceran tres ventanas. Haz click sobre la que pone **Relleno** y selecciona la primera opcion (la que parece una X pequeñita). Acto seguido, hazclick sobre la ventana que pone **Color de trazo** y selecciona la segunda opcion (la que parece un cuadrado azul). Verás como tu imagen aparece dibujada solo con su perfil. Esta es la imagen que buscamos.

<img width="1920" alt="acb" src="https://user-images.githubusercontent.com/75345847/172210035-0d7eba09-926d-4e9c-b958-3048669347ab.png">
<img width="299" alt="acb" src="https://user-images.githubusercontent.com/75345847/172210465-a140c266-01b6-4612-a2d5-e1db7c4dfa0a.png">
<img width="297" alt="acb" src="https://user-images.githubusercontent.com/75345847/172210526-21d9c739-54f9-4ab4-9224-fe77ed2a470e.png">

> **5º paso:** Asegurate de que esta nueva imagen esta bien dentro del lienzo. Si tienes dudas, puedes hacer más grande el lienzo, tal y como aparece en las imagenes de debajo, y garantizar que ninguna seccion de la imagen queda fuera de los margenes.

<img width="1920" alt="acb" src="https://user-images.githubusercontent.com/75345847/172210759-d663cf1f-2d3e-4875-bfe9-02875c0bebba.png">
<img width="612" alt="acb" src="https://user-images.githubusercontent.com/75345847/172210873-e48ca3f9-3864-49dc-884b-931c5c9000e5.png">

> **6º paso:** Exporta la imagen en formato **png**.

<img width="1916" alt="acb" src="https://user-images.githubusercontent.com/75345847/172210993-ee601c60-05b8-4e95-a33f-d1c1d1012b9b.png">

> **7º paso:** Abre el programa **LigthBurn**, y sincroniza la impresora. Recuerda que debes conectar el Arduino a tu ordenador. Cuando configures esto la primera vez, ya no tendrás que volver a hacerlo; automaticamente, el programa reconocerá la impresora sin necesidad de que la vuelvas a configurar. Al mismo tiempo, aprovecha para configurar los parametros de la CNC para que despues no tengas ningun problema.

```
Como LightBurn es un programa de pago, y al haber consumido el periodo de prueba gratuita 
no he podido hacer capturas acerca de cómo crear la máquina dentro del programa, 
os dejo varios videos sacados de Youtube que lo explican muy bien.
```

[Creacion de la maquina](https://www.youtube.com/watch?v=xUgUD4QHlmg) // [Ajustes del programa](https://www.youtube.com/watch?v=PWLe0bZlu6E) // [Ajustes de la maquina](https://www.youtube.com/watch?v=rpV7bDHyYjE)

> **8º paso:** Importa la imagen que has hecho antes en InkScape, y dale a **Iniciar**. La CNC debería empezar a funcionar, y a imprimir tu imagen. 

<img width="947" alt="acb" src="https://user-images.githubusercontent.com/75345847/172215927-d67f693a-5536-4ff9-82d3-a1beb18d40c1.png">


