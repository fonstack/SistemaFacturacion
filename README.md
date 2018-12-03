# Sistema simple de Facturación [C++]

## ***Introducción***
Sistema de facturación de una empresa de ***envíos express***, en la cual se piden los datos del *cliente y de la compra*, y se procede a emitir la *factura*.


## ***ScreenShots***

### *Bienvenida*
![Bienvenida](https://i.ibb.co/f0nzf4Q/Sistema-Facturacion1.png)

### *Factura*
![Factura](https://i.ibb.co/j3SKK5D/Sistema-Facturacion2.png)

### *Resumen del día*
![Resumen](https://i.ibb.co/vX5M3Mc/Sistema-Facturacion3.png)


## ***Especificaciones de desarrollo***
> Software desarrollado con el IDE *DevC++*, en el lenguaje ***C++***


## ***Especificaciones del Sistema***
Una empresa de envíos express, ofrece los servicios de despacho de encomiendas a cualquier parte del mundo. La compañía cuenta con un sistema de facturación que no cumple con lo establecido en la Gaceta Oficial N° 41.239 acerca del IVA. En este sentido, se le solicita a usted desarrolle un programa en C, que permita cumplir con la normativa vigente.

Para procesar cada factura, se conoce el código del cliente, el tipo de encomienda: Documento (“D”) o Paquete (“P”) y el peso de la encomienda en Kg. Cuando sea paquete (caja), se debe solicitar: el ancho, alto y profundidad de la caja en centímetros, lo cual permite calcular el peso volumétrico. Adicionalmente se conoce también el código del medio de pago a ser utilizado, el cual podrá ser: Medios Electrónicos (“M”) o Efectivo (“E”).

El programa debe determinar si el peso volumétrico ((alto*ancho*profundidad) / 5000) en caso de que sea paquete, es mayor que el peso del paquete y aplicar las siguientes tarifas en función al peso más alto de los 2:
- Documentos Bs. 62.515 hasta 1 kg y Bs. 35.904 por cada medio kilogramo adicional (No aplica peso volumétrico).
- Paquete Bs. 115.579 hasta 2 kg y Bs. 25.080 por cada medio kilogramo adicional.
#### Normativa Gaceta Oficial N° 41.239 acerca del IVA:
- Siempre Facturar con 12 % de IVA si la forma de pago es efectivo
Si la forma de pago es Medio Electrónico:
- Facturar con 9 % de IVA si el monto a facturar en menor o igual a Bs. 2.000.000
Facultad de Ingeniería
PROYECTO I 1718-1 Algoritmos y Programación
- Facturar con 7% de IVA si el monto es superior a Bs. 2.000.000
- 
Se desean procesar estas informaciones a lo largo del día en los Centro de Atención al Cliente y determinar lo siguiente:

* Para cada Encomienda, el Programa deberá Desplegar la Información de la Guía con los siguientes datos:
  * El código del Cliente
  * El Peso de la Encomienda
  * El Tipo de Encomienda “Documento” o “Paquete”
  * El Peso Volumétrico (en caso de que aplique)
  * El Tipo de Pago “Electronico” o “Efectivo”
  * El Monto a Pagar (sin IVA - SubTotal)
  * El Monto del IVA, indicando si es 7%, 9% o 12 %
  * El Monto Neto a Pagar (incluye el IVA - Total)

* Al final del Día.
  * La cantidad total de facturas del día
  * La cantidad total de facturas por Tipo de Encomienda
  * El Paquete más pesado indicando, Código de Cliente, Monto Neto Pagado y Kg
  * El Paquete con menor peso volumétrico indicando Código de Cliente, Monto Neto Pagado, peso volumétrico en Kg y peso del paquete
  * El Monto Total Neto Facturado (incluyendo IVA)
  * El Monto Total de IVA cobrado, independientemente si fue 7%, 9% o 12%
  * El Promedio de Pago de todos los Clientes por Tipo de Encomienda

El programa deberá efectuar todas las validaciones requeridas, desplegar mensajes de error, hacer uso de programación estructurada, utilizando funciones void y no void, así como pase de parámetros por valor y por referencia.