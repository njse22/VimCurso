# Edición de Texto

Para editar un archivo de texto en Vim debemos entrar al modo *INSERT* para ello debemos presionar la tecla *i* nos daremos cuenta de que estamos en este modo porque en la parte inferior izquierda del editor.

<img src="figuras/vi8.gif" title="" alt="Figura 8. modo de insert en vim" data-align="center">

En este modo podremos empezar a editar partir del lugar donde esté ubicado nuestro cursor; en caso tal de que queramos editar algo justo después del lugar donde está ubicado nuestro cursor lo haríamos presionando la tecla *a*, ahora bien si queremos editar desde el final de la línea de texto lo hacemos con *shif + a* (con la 'a' mayúscula) esto ubicará nuestro cursor al final de la línea como se ve en la siguiente imagen:

<img src="figuras/vi9.gif" title="" alt="Figura 9. insertal al final de la linea en vim" data-align="center">

Supongamos que quieres agregar una nueva linea de comentario a tu código, esto lo puedes hacer con  la tecla *o* para agregar una nueva linea **debajo** de la línea en la cual se encuentra el cursor y *O* ('*O*' mayúscula) para agregar una línea **arriba** de donde está el cursor

<img src="figuras/vi37.gif" title="" alt="" data-align="center">

Para eliminar texto **en el modo normal** lo haremos con presionando la tecla *x*

<img src="figuras/vi10.gif" title="" alt="Figura 10. eliminar texto en modo normal" data-align="center">

También puedes eliminar toda una línea de texto con *d + d* como se ve en la siguiente imagen:

<img title="" src="figuras/vi14.gif" alt="Figura 14. eliminar toda una linea de texto en Vim" data-align="center">

Si no quieres eliminar toda una línea si no lo que esta delante de una palabra por ejemplo puedes hacerlo con *d + shif + 4* (o lo que es lo mismo buscar la combinación de teclas *d + $*), que elimina todo lo que este delante del cursor, la siguiente imagen lo muestra un poco mejor:

<img src="figuras/vi15.gif" title="" alt="Figura 15. eliminar después del cursor" data-align="center">

Antes te dije que podías navegar con las teclas *w, b, e* bueno con ellas también puedes eliminar; para eliminar la palabra (o fracción de ella) que esta **delante del cursor** puedes usar *d + w*

<img src="figuras/vi19.gif" title="" alt="Figura 19. d + w en vim" data-align="center">

con *d + b* eliminas la palabra que este **antes del cursor**

<img src="figuras/vi20.gif" title="" alt="Figura 20. d + b" data-align="center">

Supongamos ahora que quieres eliminar una cantidad *'n'* de palabras que están **delante de los cursos** ¿cómo lo harías?, muy sencillo *d + 'n' + w*, es decir si yo quiero eliminar las cuatro palabras que están delante de mi cursor lo puedo hacer con *d + 4 + w*, como se ve en la siguiente imagen:

<img src="figuras/vi21.gif" title="" alt="Figura 21. eliminar n palabras en vim" data-align="center">

Esta demás decir que si lo que quieres es eliminar *'n'* palabras que están **antes del cursor** lo podrías hacer con *d + 'n' + b*.

Quizá te estés preguntando, si puedes copiar/cortar y pegar y la respuesta es claramente si, pero veamos como puedes hacerlo desde el **modo normal**, todas las opciones que te acabo de mostrar para eliminar, son en realidad una opción de *cortar* y para *pegar* usamos la tecla *p* y *Shif + p* (es decir la *'P'* mayúscula), veamos esto con un ejemplo supongamos que queremos *cortar y pegar* una línea de texto, ya vimos que con *d + d* podemos *"eliminar"* (ahora sabemos que en realidad es *cortar*) toda una línea de texto; en la siguiente imagen usamos la tecla *p* para pegar la línea **después de** la línea donde esta nuestro cursor.

<img src="figuras/vi22.gif" title="" alt="Figura 22. cortar y pegar en Vim" data-align="center">

En caso tal que queramos *pegar* **antes de** la línea donde esta nuestro cursor lo haremos con *P*.

<img src="figuras/vi23.gif" title="" alt="Figura 23. copiar y pegar en vim" data-align="center">

Ahora veamos la opción de copiar, para copiar un texto primero debemos seleccionarlo, ¿cómo seleccionamos texto en Vim? Para esto existe el modo *Visual* en el cual entramos con la tecla *v*

<img src="figuras/vi37.gif" title="" alt="" data-align="center">

Estando en este modo podremos seleccionar texto con sólo mover nuestro cursor

<img src="figuras/vi35.gif" title="" alt="" data-align="center">

Una vez seleccionado el texto podremos copiarlo con la tecla *y* y pegarlo de la misma forma que hemos visto antes con la tecla *p*

<img src="figuras/vi36.gif" title="" alt="" data-align="center">

Quizá en algún momento quieras copiar todo el contenido de un archivo de texto diferente a archivo en el que estas, esto lo puedes hacer con *:r archivo* lo que copiara el contenido de *archivo* en tu archivo actual.

<img src="figuras/vi38.gif" title="" alt="" data-align="center">

Nota: más adelante en *Algunos comandos de Vim* veremos como seleccionar lineas especificar del texto con *:r* (para Linux).

En el [siguiente capitulo](capitulo4.md) veremos los comandos undo and redo. 
