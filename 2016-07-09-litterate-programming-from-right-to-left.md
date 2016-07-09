```
pushd /Users/emir/spaces/emigspace/emig.github.io/ # we go to blog the dir
entry="`date +%Y-%m-%d-$1.md`"                     # setups a blog entry file name with jekyll format
touch $entry
vi $entry                                          # we start editing
git add $entry                                     # we ended editing
git commit -am "added entry"
popd                                               # we go back to the origin
```

El bloque de comentarios tendría que estar del lado izquierdo
pero no existe un operador que me permita entrar desde el modo
comentario al modo programa, como si lo hay en el sentido contrario.

En castellano lo natural es leer de izquierda a derecha.
Los comentarios al código tendrían que acompañar a éste al lado
izquierdo del mismo.

Una manera de conseguir este efecto es comentar cada linea de código
DESPUÉS, y hacer que cada línea se una a la anterior con un macro de vim,
por ejemplo. La primera solución que se me ocurre necesita de una edición temporal.
