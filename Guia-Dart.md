# Guia Dart
## Estructura de proyecto
`.dart_tool` : Configuración de Dart (No tocar)  
`bin` : Clases(No tan recomendado) y método principal  
`lib` : Lógica y clases  
`test` : Clases de test  

## Variables y tipo de datos
Sintaxis:  
`tipo nombre = valor`  
Ejemplo:  
`int X = 10`  
`String cadena = 'Hola'`

Existen en dart las variables dinámicas: 
- En tiempo de compilación : `var` . Una vez se asigne el tipo de dato,no puede cambiar  
- En tiempo de ejecución : `dynamic` . Permite pasarle otros tipos de datos 

## Comentarios
`/** ... */` : Documentación
`/* ... */` : Varias líneas  
`// ...` : Una línea

## StringBuffer
`StringBuffer buffer = StringBuffer();` Permite almacenar cadenas

## Listas
En Dart no existen arreglos,pero si listas.  
`List<tipo> lista = [];`

