[Volver](https://github.com/cristianfloresee/Libreta-GIT)

This is intended as a quick reference and showcase. For more complete info, see [John Gruber's original spec](http://daringfireball.net/projects/markdown/) and the [Github-flavored Markdown info page](http://github.github.com/github-flavored-markdown/).

Note that there is also a [Cheatsheet specific to Markdown Here](./Markdown-Here-Cheatsheet) if that's what you're looking for. You can also check out [more Markdown tools](./Other-Markdown-Tools).

## Tabla de Contenidos
 - [1. Encabezados](#encabezados)
 - [2. Énfasis](#2-características)
 - [3. Listas](#use-cases)
 - [4. App Preview](#app-preview)
 - [5. Deploying](#5-deploying)


## Encabezados

```no-highlight
# H1
## H2
### H3
#### H4
##### H5
###### H6
```

# H1
## H2
### H3
#### H4
##### H5
###### H6


## Énfasis

| Resultado | MarkDown |
| -- | -- |
| *cursiva* | `*cursiva*` | 
| **negrita** | `**negrita**` | 
|  __negrita__ | `__negrita__` |
|  ~~tachado~~ | `~~tachado~~` |


```no-highlight
Combinación de negrita y cursiva: **negrita y _negrita y cursiva_**.
```


## Listas

```no-highlight
Lista numerada (ordenada)

1. Este es el primer elemento
2. Este es el segundo elemento
3. Este es el tercer elemento
```
Lista numerada (ordenada)

1. Este es el primer elemento
2. Este es el segundo elemento
3. Este es el tercer elemento

***

```no-highlight
Lista de puntos (desordenada)

* Un elemento de la lista
* Otro elemento de la lista
* El tercer elemento de la lista
```

Lista de puntos (desordenada)

* Un elemento de la lista
* Otro elemento de la lista
* El tercer elemento de la lista

***

```no-highlight
Se pueden emplear también + y - en vez de *

* Un elemento de la lista
+ Otro elemento de la lista
- El tercer elemento de la lista
```

Se pueden emplear también + y - en vez de *

* Un elemento de la lista
+ Otro elemento de la lista
- El tercer elemento de la lista

***

```no-highlight
Se pueden mezclar distintos tipos de listas y anidar unas dentro de otras.

1. Esto es una lista ordenada
2. Segundo elemento de la lista ordenada
    1. Esta es una lista ordenada anidada dentro de otra
        * Lista desordenada anidada a tercer nivel
        * Segundo elemento de esta lista
    2. Este es el segundo elemento de la lista ordenada anidada
```

Se pueden mezclar distintos tipos de listas y anidar unas dentro de otras.

1. Esto es una lista ordenada
2. Segundo elemento de la lista ordenada
    1. Esta es una lista ordenada anidada dentro de otra
        * Lista desordenada anidada a tercer nivel
        * Segundo elemento de esta lista
    2. Este es el segundo elemento de la lista ordenada anidada

## Párrafos

Para crear párrafos se deja una línea en blanco.
Este es el primer párrafo.

Este es el segundo párrafo

***

Para hacer un salto de línea de sejan 2 espacios en blanco al final de la última palabra de esa línea.
Este es el primer párrafo.  
Este es el segundo párrafo

## Links

```no-highlight
[Enlace](https://github.com/cristianfloresee)
```
[Enlace](https://github.com/cristianfloresee)

***

```no-highlight
[Enlace 1][1], [Enlace 2][2], [Enlace 3][3]

[1]: https://github.com/cristianfloresee
[2]: https://github.com/cristianfloresee
[3]: https://github.com/cristianfloresee
```
[Enlace 1][1], [Enlace 2][2], [Enlace 3][3]

[1]: https://github.com/cristianfloresee
[2]: https://github.com/cristianfloresee
[3]: https://github.com/cristianfloresee

***

```no-highlight
<https://github.com/cristianfloresee>
```
<https://github.com/cristianfloresee>


## Citas

```no-highlight
Esto es una línea normal

> Esto es parte de un bloque de cita.
> Esto es parte del mismo bloque de cita.
```

Esto es una línea normal

> Esto es parte de un bloque de cita.
> Esto es parte del mismo bloque de cita.

***

```no-highlight
> Esto es parte de un bloque de cita.
Esto continúa el bloque incluso aunque no hay símbolo 'mayor que'.

La línea en blanco finaliza el bloque.
```

> Esto es parte de un bloque de cita.
Esto continúa el bloque incluso aunque no hay símbolo 'mayor que'.

La línea en blanco finaliza el bloque.

Esto es una línea normal

***

```no-highlight
> Esto es parte de un bloque de cita.
> Esto es parte del mismo bloque de cita.
>
> > Esto es otro bloque de cita anidado.
> > Esto es parte del bloque anidado.
>
> Esto es parte del bloque de cita de primer nivel.
```

> Esto es parte de un bloque de cita.
> Esto es parte del mismo bloque de cita.
>
> > Esto es otro bloque de cita anidado.
> > Esto es parte del bloque anidado.
>
> Esto es parte del bloque de cita de primer nivel.

## Líneas Horizontales

```no-highlight
***
```

***

```no-highlight
- - -
```

- - -

```no-highlight
___
```

___

## Carácteres Especiales

| Resultado | MarkDown |
| -- | -- |
| \| |  `\|` | 
| \\ |`\\` | 
| \` | ` \` ` | 


```no-highlight
\*  
\_  
\{  
\}  
\[  
\]  
\(  
\)  
\#  
\+  
\-  
\.  
\!  
\:  
\|
```

\\  
\`  
\*  
\_  
\{  
\}  
\[  
\]  
\(  
\)  
\#  
\+  
\-  
\.  
\!  
\:  
\|


## Tablas 
```
Cabecera | Cabecera | Cabecera
-------|--------|-------
Celda | Celda | Celda
Celda | Celda | Celda
```

Cabecera | Cabecera | Cabecera
-------|--------|-------
Celda | Celda | Celda
Celda | Celda | Celda

## Código Fuente

```apache
<VirtualHost *:80>
DocumentRoot /www/example1
ServerName www.example1.com

# Other directives here

</VirtualHost>
```

```c
#include <stdio.h>
int main()
{
    printf("¡Hola, mundo!\n");
    return 0;
}
```

```javascript
function fancyAlert(arg) {
  if(arg) {
    $.facebox({div:'#foo'})
  }
}
```

```python
s = "Python syntax highlighting"
print s
```

```ruby
require 'redcarpet'
markdown = Redcarpet.new("Hello World!")
puts markdown.to_html
```

```mysql
SELECT 'HOLA MUNDO';
```


## Emojis

| :bowtie: `:bowtie:` | :smile: `:smile:` | :laughing: `:laughing:` |
|---|---|---|
| :blush: `:blush:` | :smiley: `:smiley:` | :relaxed: `:relaxed:` |
| :smirk: `:smirk:` | :heart_eyes: `:heart_eyes:` | :kissing_heart: `:kissing_heart:` |
| :kissing_closed_eyes: `:kissing_closed_eyes:` | :flushed: `:flushed:` | :relieved: `:relieved:` |
| :satisfied: `:satisfied:` | :grin: `:grin:` | :wink: `:wink:` |
| :stuck_out_tongue_winking_eye: `:stuck_out_tongue_winking_eye:` | :stuck_out_tongue_closed_eyes: `:stuck_out_tongue_closed_eyes:` | 

## Youtube

```html
<a href="http://www.youtube.com/watch?feature=player_embedded&v=ID_VIDEO_YOUTUBE" target="_blank">
    <img src="http://img.youtube.com/vi/ID_VIDEO_YOUTUBE/0.jpg" alt="IMAGE ALT TEXT HERE" width="240" height="180" border="10"/>
</a>
```