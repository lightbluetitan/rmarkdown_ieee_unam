---
title: "Lenguaje de Marcado Ligero"
author: "Renzo Cáceres Rossi"
date: "2022/06/14"
subtitle: Markdown - RMarkdown
institute: IEEE - UNAM
output:
  html_document:
    code_download: TRUE
---

<!-- Añadir comentarios a nuestro documento Markdown - HTML tags -->


# Sintaxis Básica Markdown

## Encabezados - Títulos

# Título 1
## Título 2
### Título 3
#### Título 4
##### Título 5
###### Título 6

## Negrita - Cursiva - Tachado - Subrayado

*Texto formateado como Negrita*

**Texto formateado como Cursiva**

~~Texto tachado~~

<u>Texto subrayado</u>

## Enlaces - Añadir links a nuestro documento Markdown

<https://www.facebook.com/IEEE.UNAM>


[IEEE - UNAM](https://www.facebook.com/IEEE.UNAM){target="_blank"}

[IEEE - UNAM](https://www.facebook.com/IEEE.UNAM "Ingresa al IEEE UNAM"){target="_blank"}


## Imágenes - Añadir imágenes a a nuestro documento Markdown

<center>

![](logo_r.png)


![](https://d33wubrfki0l68.cloudfront.net/aee91187a9c6811a802ddc524c3271302893a149/a7003/images/bandthree2.png){width=300}

</center>


## Código - Añadir código de distintos lenguajes de programación - R - Python - SQL


    summary(mtcars)
    
La función `barplot()` nos permite crear diagramas de barras (**Bar Charts**) en el lenguaje de programación R.

```
x <- table(mtcars$cyl)

colores <- c("orange","blue","purple")

barplot(x,xlab="Cilindros",ylab="Frecuencias",main="Número de Cilindros",col=colores)
```

```Python
import matplotlib.pyplot as plt
 

eje_x = ['Python', 'R', 'Node.js', 'PHP']
 

eje_y = [50,20,35,47]
 

plt.bar(eje_x, eje_y)
 

plt.ylabel('Cantidad de usuarios')
 

plt.xlabel('Lenguajes de programación')
 

plt.title('Usuarios de lenguajes de programación')
 

plt.show()
```

    SELECT id_usuario,usuario_nombre,usuario_apellidos from usuario;
    
```sql
USE Northwind;

SELECT * FROM Products;
```
