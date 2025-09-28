---
title: If, switch y cosas similares
slug: If-switch-cosas-similares
description: Breve descripcion y uso de estas estructuras de control.
longDescription: HTML is the foundation of all websites. This guide will walk you through creating your first simple website using HTML.
cardImage: "https://zaggonaut.dev/Foy.webp"
tags: [".Net", "c#", "else", "If", "switch"]
readTime: 1
featured: true
timestamp: 2007-12-19T12:17:00+06:00
---

Como todo lenguaje de prgramación de alto nivel C# tiene estructuras de control, la mas conocida es el **if**.
```C#
if (condicion) // si "condicion" es verdadero
{
    //hacer algo
}
else // si no
{
    //hacer otra cosa
}
tambien se pueda usar
if (condicion) // si "condicion" es verdadero
{
    //hacer algo
}
else if (condicion2) // si la "condicion2" es verdadero
{
    //hacer algo
}
else // si no
{
    //hacer otra cosa
}
```

Tambien estan los **switch** que se utilizan para mejorar la estructura cuando se pregunta sobre el valor de un mismo dato varias veces:

```C#
switch (letra)
{
    case ('A'):
        // hacer algo
        break;
    case ('B'):
        //hacer algo
        break;
    default:
        //hacer algo en caso de que no se cumpla ninguna condición
        break;
}
```

Hay un último caso interesante y que se da con bastante frecuencia en el cual nos interesa evaluar una condición específicamente para asignarle un valor a una variable, esto se podría hacer de la siguiente manera:

```C#
if (condicion)
{
    variable = 1;
}
else
{
    variable = 2;
}
```
o bien esta expresión que es equivalente y ocupa menos espacio:
```C#
variable = condicion ? 1 : 2;
otro ejemplo
variable = (x == 0) ? true : false;
```

esto es si x es igual a cero asignarle true a variable, si x no es cero asignarle false a variable. Muy util a mi parecer.
