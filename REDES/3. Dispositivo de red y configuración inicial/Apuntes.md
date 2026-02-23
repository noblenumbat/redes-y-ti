# Diseño de Redes Jerárquico

## Acceso, Distribución y Núcleo

### Capa de acceso

La capa de acceso proporciona un punto de conexión a la red para los dispositivos para usuarios finales y permite que varios hosts se conecten a otros hosts a través de un dispositivo de red, generalmente un conmutador, como el Cisco 2960-XR que se muestra en la figura, o un punto de acceso inalámbrico. Normalmente, la porción de red de la dirección IP será la misma para todos los dispositivos de una misma capa de acceso.

Si un mensaje está destinado a un host local, según se indique en la porción de red de la dirección IP, el mensaje permanecerá en el nivel local. Si está destinado a una red diferente, pasa a la capa de distribución. Los conmutadores proporcionan la conexión a los dispositivos de la capa de distribución, generalmente un dispositivo de Capa 3, como un enrutador o un conmutador de Capa 3.

Cisco 2960-XR

![cisco-2960](/REDES/3.%20Dispositivo%20de%20red%20y%20configuración%20inicial/Imagenes/cisco%202960-xr.png)

### Capa de Distribución

La capa de distribución proporciona un punto de conexión para redes separadas y controla el flujo de información entre las redes. Por lo general, contiene conmutadores más potentes, como la serie Cisco C9300 que se muestra en la figura, que la capa de acceso, así como enrutadores para el enrutamiento entre redes. Los dispositivos de la capa de distribución controlan el tipo y la cantidad de tráfico que circula desde la capa de acceso hasta la capa principal.

Cisco de la Serie C9300

![cisco-c9300](/REDES/3.%20Dispositivo%20de%20red%20y%20configuración%20inicial/Imagenes/C9300.jpg)

### Capa de Núcleo

La capa de núcleo es una capa troncal de alta velocidad con conexiones redundantes (de respaldo). Es la encargada de transportar grandes cantidades de datos entre múltiples redes finales. Los dispositivos de capa de núcleo suelen incluir enrutadores y conmutadores muy potentes y de alta velocidad, como el Cisco Catalyst 9600 que se muestra en la figura. El objetivo principal de la capa de núcleo es transportar datos con rapidez.

Cisco Catalyst 9600

![catalyst-9600](/REDES/3.%20Dispositivo%20de%20red%20y%20configuración%20inicial/Imagenes/Catalyst-9600.png)

# La nube y los servicios en la nube

## Computación en la nube

Generalmente cuando hablamos de la nube, hablamos de tres elementos:

- Centros de datos  
- Computación en la nube  
- Virtualización  

Los centros de datos suelen ser grandes instalaciones que proporcionan grandes cantidades de energía, refrigeración y ancho de banda. Solo empresas muy grandes pueden permitirse sus propios centros de datos. La mayoría de las organizaciones más pequeñas arrienda los servicios de un proveedor de la nube.

---

## Servicios en la nube

Los servicios en la nube incluyen lo siguiente:

- **SaaS** – Software como servicio  
- **PaaS** – Plataforma como servicio  
- **IaaS** – Infraestructura como servicio  

---

## Modelos de nube

Hay cuatro modelos de nube principales:

### Nubes Públicas
Las aplicaciones basadas en la nube y los servicios que se ofrecen en una nube pública están a disposición de la población en general.

### Nubes Privadas
Las aplicaciones y los servicios basados en una nube privada están destinados a una organización o entidad específica, como el gobierno.

### Nubes Híbridas
Una nube híbrida se compone de dos o más nubes, donde cada parte sigue siendo un objeto separado, pero todas están conectadas mediante una única arquitectura.

### Nubes Comunitarias
Una nube comunitaria se crea para el uso exclusivo de una comunidad específica. Las diferencias entre nubes públicas y nubes comunitarias son las necesidades funcionales que se personalizan para la comunidad.

---

## Virtualización

La virtualización es la base de la computación en la nube. Sin esta base, la computación en la nube que se implementa masivamente no sería posible.

La virtualización significa crear una versión virtual de algo que originalmente es físico, como una computadora.  
Un ejemplo sería ejecutar una **“computadora con Linux”** en un PC con **Windows**.

Una de las ventajas más importantes de la virtualización es un menor costo total:

- **Se requiere menos equipo**  
  La virtualización permite la consolidación de servidores, lo que requiere menos dispositivos físicos y reduce los costos de mantenimiento.

- **Menor consumo de energía**  
  La consolidación de servidores reduce los costos mensuales de alimentación y refrigeración.

- **Se requiere menos espacio**  
  La consolidación de servidores reduce la cantidad de espacio requerido.

---

## Beneficios adicionales de la virtualización

- **Simplificación de prototipos**  
  Se pueden crear rápidamente laboratorios autónomos que operan en redes aisladas para las pruebas y los prototipos de instalaciones de red.

- **Aprovisionamiento de servidores más rápido**  
  Crear un servidor virtual es mucho más rápido que aprovisionar un servidor físico.

- **Mayor tiempo de actividad del servidor**  
  La mayoría de las plataformas de virtualización de servidores ahora ofrecen funciones avanzadas de tolerancia a fallas redundantes.

- **Recuperación mejorada ante desastres**  
  La mayoría de las plataformas de virtualización de servidores empresariales tienen software que puede ayudar a probar y automatizar la computación por error antes de que ocurra un desastre.

- **Soporte de tecnologías heredadas**  
  La virtualización puede extender la vida útil de los sistemas operativos y las aplicaciones, brindando más tiempo para que las organizaciones migren a soluciones más nuevas.

---

## Hipervisor

El **hipervisor** es un programa, un firmware o un hardware que agrega una capa de abstracción sobre el hardware físico real.  
Esta capa de abstracción se utiliza para crear máquinas virtuales que tienen acceso a todo el hardware de la máquina física, como:

- CPU  
- Memoria  
- Controladores de disco  
- NIC  

Cada una de estas máquinas virtuales ejecuta un sistema operativo completo y separado.

---

## Hipervisor Tipo 1 (Bare Metal)

El hipervisor de tipo 1 también se denomina **infraestructura física (bare metal)**, porque está instalado directamente en el hardware.  

Los hipervisores de tipo 1 se usan generalmente en:

- Servidores empresariales  
- Dispositivos de red  
- Centros de datos  

---

## Hipervisor Tipo 2 (Alojado)

Un hipervisor de tipo 2 es un software que crea y ejecuta instancias de máquinas virtuales (VM).

- La computadora donde se ejecuta el hipervisor se denomina **host**.
- El hipervisor está instalado sobre un sistema operativo existente, como:
  - macOS  
  - Windows  
  - Linux  

Luego, una o más instancias adicionales de sistemas operativos se instalan sobre el hipervisor.

Una gran ventaja de los hipervisores de tipo 2 es que **no se requiere software adicional de consola de administración**.

---

# Sistema binario y decimal

```
Positional Notation - Place Value

   10^6	      10^5       10^4     10^3    10^2   10^1  10^0
-----------------------------------------------------------
1,000,000    100,000    10,000    1,000    100    10    1
__________________________________________________________
			            9       1      6    8     


	9 x 1000
	1 x 100
	6 x 10
	8 x 1
	_________
    Suma    9168

Decimal - Base 10 (0,1,2,3,4,5,6,7,8,9)

---
Binary - Base 2 (0,1)

2^7	2^6	2^5	2^4	2^3	2^2	2^1	2^0
-----------------------------------------------------------
128	 64	 32	16	 8	 4	 2	 1
__________________________________________________________
 1	0        1      0       1       0       0       0

Los bits en 1 se activan cuando el número a convertir es <= a la suma en la posición posiciones en base 2 donde hay un bit en 1.

128 	      <= 168    ? 1
128 + 64      <= 168    ? 0
128 + 32      <= 168    ? 1
128 + 32 + 16 <= 168    ? 0
128 + 32 +  8 <= 168    ? 1


	Número 168 en binario = 168 = 10101000

	1 x 128 = 128
	1 x 32	=  32
	1 x 8   =   8
	_____________
	Total	  168

---
Ejercicio: Convertir el binario 01101101 a decimal

2^7	2^6	2^5	2^4	2^3	2^2	2^1	2^0
-----------------------------------------------------------
128	 64	 32	 16	 8	 4	 2	 1
__________________________________________________________
 0	 1    1  0   1   1   0   1

	64 + 32 + 8 + 4 + 1 = 109

``` 

## Conversión de decimal a binario

Regla

Si el número decimal a convertir es >= al valor decimal en la posición del (n) octeto binario Se resta el número decimal a convertir con el valor decimal en la posición del (n) octeto binario y se pone ese bit en 1, sino entonces se pone 0 y se compara el resto con el siguiente número en el octeto.  Si el resto es cero desde el comienzo todos los octetos se configuran en 0.


```
Ejercicio 1

Valor decimal: 101

2^7	2^6	2^5	2^4	2^3	2^2	2^1	2^0
-----------------------------------------------------------
128	 64	 32	 16	 8	 4	 2	 1
__________________________________________________________
 0	 1    1  0   0   1   0   1


Ejercicio 2

Valor decimal: 126

2^7	2^6	2^5	2^4	2^3	2^2	2^1	2^0
-----------------------------------------------------------
128	 64	 32	 16	 8	 4	 2	 1
__________________________________________________________
 0	 1    1   1  1   1   1   0


Ejercicio 3

Valor decimal: 183

2^7	2^6	2^5	2^4	2^3	2^2	2^1	2^0
-----------------------------------------------------------
128	 64	 32	 16	 8	 4	 2	 1
__________________________________________________________
 1	 0    1   1  0   1   1   1 


Ejercicio 4

Valor decimal: 134

2^7	2^6	2^5	2^4	2^3	2^2	2^1	2^0
-----------------------------------------------------------
128	 64	 32	 16	 8	 4	 2	 1
__________________________________________________________
 1	 0    0   0  0   1   1   0  


Ejercicio 5

Valor decimal: 99

2^7	2^6	2^5	2^4	2^3	2^2	2^1	2^0
-----------------------------------------------------------
128	 64	 32	 16	 8	 4	 2	 1
__________________________________________________________
 0	 1    1   0  0   0   1   1   


Ejercicio 6

Valor decimal: 240

2^7	2^6	2^5	2^4	2^3	2^2	2^1	2^0
-----------------------------------------------------------
128	 64	 32	 16	 8	 4	 2	 1
__________________________________________________________
 1	 1    1   1  0   0   0   0  

``` 

![hexToDec](/REDES/3.%20Dispositivo%20de%20red%20y%20configuración%20inicial/Imagenes/hexToDec.png)

¿Cuál es el equivalente hexadecimal de 202?

``` 
Primero convierto a binario

2^7	2^6	2^5	2^4	2^3	2^2	2^1	2^0
-----------------------------------------------------------
128	 64	 32	 16	 8	 4	 2	 1
__________________________________________________________
 1	 1    0   0  1   0   1   0  

Despues convierto a hexadecimal

2^3	2^2	2^1	2^0	| 2^3	2^2	2^1	2^0
-----------------------------------------------------------
 8	 4	 2	 1  |  8	 4	 2	 1
-----------------------------------------------------------
 1   1   0   0     1	 0	 1	 0
__________________________________________________________
         C              A  Si el valor sobrepasa a 9 se emplean letras

Dec 202 =  CA 
``` 

¿Cuál es el equivalente hexadecimal de 254?

``` 
Primero convierto a binario

2^7	2^6	2^5	2^4	2^3	2^2	2^1	2^0
-----------------------------------------------------------
128	 64	 32	 16	 8	 4	 2	 1
__________________________________________________________
 1	 1    1   1  1   1   1   0  

Despues convierto a hexadecimal

2^3	2^2	2^1	2^0	| 2^3	2^2	2^1	2^0
-----------------------------------------------------------
 8	 4	 2	 1  |  8	 4	 2	 1
-----------------------------------------------------------
 1   1   1   1     1	 1	 1	 0
__________________________________________________________
         F              F  Si el valor sobrepasa a 9 se emplean letras

Dec 254 = FE  

```

¿Cuál es el equivalente decimal de A9?

``` 
 16³      16²     16¹     16⁰
 -------------------------------
 4096     256     16       1

1. Primero se escribe la notación posicional, luego se insertan los simbolos hexadecimales debajo del valor correspondiente.

 16¹  16⁰
 --------
 16    1
 ________
  A    9

2. Multiplicar cada simbolo hexadecimal por el valor de lugar que es inferior y sumar los resultados juntos.

  (A x 16)  + (9 x 1)
  (10 x 16) + (9 x 1)
     160    +    9

Hex A9 =  169

```

> ![Note]
> 
> Es más fácil convertir el hexadecimal a decimal o valor decimal a binario primero, que convertir el número binario a decimal o hexadecimal a decimal.

```
¿Cuál de los siguientes es el equivalente decimal de 7D?

 16¹  16⁰
 --------
 16    1
 ________
  7    D

 (7 x 16) + (D x 1)
 (7 x 16) + (D x 1)
   112    +   13

 Hex 7D = 125 

```

# Tools
## OUI Lookup Tool

https://www.wireshark.org/tools/oui-lookup.html

Permite identificar el fabricante de una NIC con los tres primer bytes

## Wireshark

Ejercicio

Capturar y analizar los datos ARP locales.
  
    Conociendo mi dirección IP y MAC

  ![ip_addr_show](/REDES/3.%20Dispositivo%20de%20red%20y%20configuración%20inicial/Imagenes/ip_addr_show.png)

    direccion ip:   192.168.80.127
  
    dirección MAC:  32:68:a6:94:b5:4f
  
    dirección ip gateway: 192.168.80.1

Comenzar a capturar datos
    Seleccionar la interfaz de red para capturar paquetes
    Escribir arp en el campo de filtro

  ![captura_paq](/REDES/3.%20Dispositivo%20de%20red%20y%20configuración%20inicial/Imagenes/captura_paq.png)

    Más abajo se puede visualizar las direcciones MAC de origen y destino.

  ![src_dst](/REDES/3.%20Dispositivo%20de%20red%20y%20configuración%20inicial/Imagenes/src_dst.png)

# Tipos de direcciones MAC

## MAC de unidifusión 

Se identifica por el primer bit de la dirección MAC.

Regla fundamental 

Último bit del primer byte

  0  -> Unidifusión (unicast)
  1  -> Multidifusión (multicast)

00-07-E9-42-AC-28

Primer byte: 00

En binario:

00 = 00000000
          ↑


## MAC de multicast

01-00-5E-00-00-C8

Primer byte: 01

En binario:

01 = 00000001
          ↑

## Resumen

| MAC                 | Tipo      | Por qué     |
| ------------------- | --------- | ----------- |
| `01-00-5E-...`      | Multicast | Bit LSB = 1 |
| `00-07-E9-...`      | ✅ Unicast | Bit LSB = 0 |
| `33-33-...`         | Multicast | IPv6        |
| `FF-FF-FF-FF-FF-FF` | Broadcast | Todos 1     |

## Truco mental ultra rápido

👉 Si empieza por:

00, 02, 04, 06 → normalmente unicast

01, 33 → multicast

FF → broadcast

---

# ¿Cómo funciona un servidor DNS?

![paso-1](/REDES/3.%20Dispositivo%20de%20red%20y%20configuración%20inicial/Imagenes/DNS%20Paso1.png)
![paso-2](/REDES/3.%20Dispositivo%20de%20red%20y%20configuración%20inicial/Imagenes/DNS%20Paso2.png)
![paso-3](/REDES/3.%20Dispositivo%20de%20red%20y%20configuración%20inicial/Imagenes/DNS%20Paso3.png)
![paso-4](/REDES/3.%20Dispositivo%20de%20red%20y%20configuración%20inicial/Imagenes/DNS%20Paso4.png)
![paso-5](/REDES/3.%20Dispositivo%20de%20red%20y%20configuración%20inicial/Imagenes/DNS%20Paso5.png)

Algunos registros DNS:

A - Una dirección IPv4 de un dispositivo final

NS - Un servidor de nombre autoritativo

AAAA - Una dirección IPv6 de un dispositivo final (pronunciado quad-A)

MX - Un registro de intercambio de correo

# Mensajes DHCP

Cuando un dispositivo configurado con DHCP e IPv4 se inicia o se conecta a la red, el cliente transmite un mensaje de detección de DHCP (DHCPDISCOVER) para identificar cualquier servidor de DHCP disponible en la red. Un servidor de DHCP responde con un mensaje de oferta de DHCP (DHCPOFFER), que ofrece una concesión al cliente. El mensaje de oferta contiene la dirección IPv4 y la máscara de subred que se deben asignar, la dirección IPv4 del servidor DNS y la dirección IPv4 del gateway predeterminado. La oferta de concesión también incluye la duración de esta.

![Mensajes-DHCP](/REDES/3.%20Dispositivo%20de%20red%20y%20configuración%20inicial/Imagenes/Mensajes%20DHCP.png)

# PUERTOS

PUERTO | PROTOCOLO | APLICACION
-------|-----------|------------ 
20		 | TCP       |  FTP Datos
21		 | TCP       |  FTP Control
22		 | TCP       |  SSH
23		 | TCP       |  Telnet
25		 | TCP       |  SMTP
53	   | UDP/TCP	 |  Servidor de nombres de dominio
67	   | UDP		   |  DHCP Servidor
68	   | UDP		   |  Cliente
69	   | UDP		   |  TFTP Protocolo trivial de transferencia de archivos
80	   | TCP		   |  HTTP
110    | TCP       |  POP3
143    | TCP       |  IMAP 
161    | UDP       |  SNMP
443    | TCP       |  HTTPS
