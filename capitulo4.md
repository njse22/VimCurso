# Deshacer y rehacer (undo y redo)

Ahora que ya sabemos un poco más del uso de Vim, veamos como podemos deshacer y rehacer texto, el primero se hace simplemente con la tecla *u*

<img src="figuras/vi16.gif" title="" alt="Figura 16. undo en vim" data-align="center">

Si por casualidad quieres devolverte a un cambio en el cual hiciste x cantidad de cambios puedes ver la *undolist*, estando **en el modo normal** escribe *:undolist*

<img src="figuras/vi17.gif" title="" alt="Figura 17. Undolist" data-align="center">

En esta lista se encuentran los cambios realizados sobre el archivo ordenados desde el menos reciente al más reciente de arriba hacia abajo, fíjate en las columnas de la lista etas son de izquierda a derecha *number*, número o identificador del cambio; *changes*, o cantidad de cambios realizados; *when*, que especifica cuando se realizó el cambio; si lo que quieres es devolverte a un cambio especifico lo que debes hacer es escribir *:undo N* donde *N* es el número o identificador del cambio.

<img src="figuras/vi18.gif" title="" alt="Figura 18. undo N" data-align="center">

Anterior mente habíamos hablado de *Buffers* en las acciones de Vim, con *undo* y *redo* pasa lo mismo si quieres volver al **cambio deshecho anterior** (redo) lo puedes hacer con *Ctrl + r*.

En el [siguiente capitulo](capitulo5.md) veremos como Remplazar y cambiar palabras.
