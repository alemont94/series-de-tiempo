# Universidad Autónoma del Estado de México
# Series de Tiempo
# 2 de febrero de 2017
#Practica 1. Introducción a R

#R es sensible a mayúsculas y minúsculas (case sensitive)

x <- 1:25 
# Genera un vector llamado “x” que va de uno en uno desde 1 hasta 25
x

mean(x) 
# Da la media del vector x
meAn(x) 
#Indica un error (rectificando que es sensible a las mayúsculas)

y <- 2:38
y

#Para conocer el listado de los objetos que hemos creado se utiliza ls()
ls()

#Definiendo vectores en R
x2 <- c(2,4,6,8)        
# El símbolo “<- “se denomina vector de asignación
x2
x3 <- c(2,4,5,7,8,1000)
x3
a <- 1:23
b <- 1:100
y <- seq(8,80,4)      
#Creo una secuencia de 8 a 80 con intervalo que va de 4 en 4 
y
length(x)             
#Para conocer la longitud de un vector
length(y)

#CALCULO MANUAL DE LA MEDIA
?sum 
# “sum” es una función de R que calcula la suma de los valores en un vector

media <- sum(x)/length(x)   
# Es el cálculo “manual” de la media del vector x, suma(x)/n, en este caso length nos da n 

mean(x)
media
# Comprobando que mean(x)=media

# Para remover o eliminar alguna variable creada se utiliza la función “rm()”
rm(x4)
ls() #Comprobando que se borró x4

rm(list=ls())
# Borra todo del environment, o sea, todas las variables creadas

# También se pueden crear vectores con valores string 
nse<-c(“alto”, “medio”, “bajo”)

x<-rnorm(100)
#Densidad, función de distribución, función cuantitativa y generación aleatoria para la distribución normal con media igual a media y desviación estándar igual a sd.
x
plot(x)
# “plot(x)” genera la gráfica de x

#CALCULO MANUAL DE LA DESVIACION ESTANDAR
sd(x)               
# Función para calcular la desviación estándar de x
var(x)              
# Función para calcular la varianza de x
# A partir de la función “var(x)” se calcula la desviación estándar de la siguiente manera:
sqrt (var(x))   
# Dónde “sqrt()” es una función que calcula la raíz cuadrada, en este caso la raíz cuadrada de la varianza de x.



# Creamos “y” que es igual a “x” más otros valores simulados

y=x+rnorm(100, mean=50,sd=0.5) 

# Dónde:
# Se está calculando la normal de 100, con media 50 y desviación estándar de 0.5 (sd es desviación estándar)

cor(x,y)
# Calcula la correlación existente entre “x” y “y”
# En este caso la correlación es muy alta porque en la ecuación de “y” se incluye a “x”.

#INDEXANDO UN VECTOR
x <- c(70,80,90,-70,-80,-90)
x[1]

x[6]

x[2:5]
# “x[ ]” Te permite ver el valor que tiene el vector “x” en la casilla “1”, “6”, y en las casillas que van desde 2 a 5 (2,3,4,5) 

x[-1]               
#Imprime todos menos el primer número o valor del vector 
x[-2:-4]
# Imprime todos los valores menos los que van en las casillas de 2 a 4 (2, 3, 4)

#ARITMETICA DE VECTORES
y <- c(0,-98,3,45,37,1,-700)
y
4*y
# Multiplica cada valor del vector por el número 4
3.1416+y 
# Suma 3.1416 a cada valor de “y”
pi + y
y^3
# Eleva al cubo cada elemento del vector

#OPERADORES RELACIONALES
# < menor que
# > mayor que
# <= menor o igual que
# >= mayor o igual que
# == igual que 
# != diferente 
8==7.99999 
# Da “false” como resultado 
8==7.99999999999999999999999999999999999999999999999999999999999999999999999999999
# Da “true” porque la diferencia es minúscula

x <- 17
x>=12 
# Esta afirmación es cierta, por eso da “true” como resultado 
x==1
# Da “false” com resultado porque es uma afirmación falsa
x!=0 “true”

a <- c(6,7,12,56,3,490)
a
a>7 
a>=16

# Te arroja los casos en los que “a” es mayor que 7, mayor o igual a 16 

a[a > 10]
# Muestra sólo los valores de “a” que sean mayores a 10

#OPERADORES LOGICOS: &, |
# "&" implica “y” o “^”, "|" implica “o” o “v”

a <- (1:25)
a
b <- (30:56)
b
x <- (101:125)
x
