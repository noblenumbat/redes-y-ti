# 15. Convertir versión de evaluación a versión completa

**Ver la versión actual de Windows Server**

Desde cmd:

``` 
DISM /online /Get-CurrentEdition
```  
---

**Asignando una clave KMS para pruebas. Del mismo modo se puede aplicar una llave de pago.**

``` 
DISM /online /Set-Edition:ServerStandard /ProductKey:WC2BQ-8NRM3-FDDYY-2BFGV-KHKQY /AcceptEula
``` 
---

# 18. Catalogo de Microsoft Update

Descarga de actualizaciones acumulativas para instalarlas de forma manual

Este es el link: https://www.catalog.update.microsoft.com/Home.aspx

Requisito: 

+ Saber cual es el KB a buscar 
+ Elegir la versión del sistema operativo
+ Elegir x86 | x64

---
# Datos red de laboratorio

PC Servidor
``` 
INTERFAZ WAN

IP          :   10.0.2.15
SUBRED      :   /24
GATEWAY     :   10.0.2.2
DNS         :   10.0.2.3

INTERFAZ LAN

IP          :   192.168.0.3
SUBRED      :   /24
GATEWAY     :   
DNS         :   
``` 

PC Cliente
``` 
IP          :   192.168.0.5
SUBRED      :   /24
GATEWAY     :   
DNS         :   
``` 
