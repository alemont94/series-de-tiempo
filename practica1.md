# series-de-tiempo
Clase UAEM
#Practica 1. Introduccion a R
#R es sensible a mayusculas y minusculas (case sensitive)
x <- 1:25
mean(x)
meAn(x)
#Indica un error

y <- 2:38
y

#Para conocer el listado de los objetos hemos creado se utiliza ls()
ls()

#Definiendo vectores en R
x2 <- c(2,4,6,8)        # El simbolo <- se denomina vector de asignacion
x2
x3 <- c(2,4,5,7,8,1000)
x3
a <- 1:23
b <- 1:100
y <- seq(8,80,4)      #Creo una secuencia de 8 a 80 con intervalo 4 
y

length(x)             #Para conocer la longitud de un vector
length(y)

#CALCULO MANUAL DE LA MEDIA 
mean(x)               #Funcion en R
media <- sum(x)/length(x)   #Manual
media

#CALCULO MANUAL DE LA DESVIACION ESTANDAR 
sd(x)               #Funcion en R
var(x)              #Funcion en R
sqrt (var(x))   #Manual

#INDEXANDO UN VECTOR
x <- c(70,80,90,-70,-80,-90)
x[1]
x[6]
x[2:5]

x[-1]               #Con indices negativos se excluyen elementos
x[-2:-4]

#ARITMETICA DE VECTORES
y <- c(0,-98,3,45,37,1,-700)
y
4*y
3.1416+y
pi + y
y^3

#OPERADORES RELACIONALES: <, >, >=, <=, ==, !=
8==7.99999
x <- 17
x>=12
x==1
x!=0

a <- c(6,7,12,56,3,490)
a
a>7
a>=16
a[a > 10]  
  
#OPERADORES LOGICOS: &, |
a <- (1:25)
a
b <- (30:56)
b
x <- (101:125)
x
#OPERADORES RELACIONALES: <, >, >=, <=, ==, !=
8==7.99999
x <- 17
x>=12
x==1
x!=0

a <- c(6,7,12,56,3,490)
a
a>7
a>=16
a[a > 10]  
a[a==3 | a<=11] 
