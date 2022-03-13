@Author : Miguel Angel Manuttupa Ligas
@Contact : manuttupa.ligas@gmail.com

# Microsoft Azure Certified AZ-900 Fundamentals
  - [Introducción](#introducción)
  - [Temario](#temario)
  - [Cómputo en la Nube](#cómputo-en-la-nube)
    - [Máquinas virtuales (Cómo servicio)](#máquinas-virtuales-cómo-servicio)
    - [Contenedores](#contenedores)
    - [Serverless](#serverless)
  
## Introducción 
El examen consta de 6 módulos importantes
1. Describir los conceptos de la nube
2. Describir los servicios centrales de Azure
3. Describir las soluciones y las herramientas de administración de Azure
4. Describir las características principales de seguridad y seguridad en la red
5. Describir las características de gobernanza, identidad, privacidad y cumplimiento
6. Describir la administración de costos de Azure y los SLA(Acuerdo de nivel de servicio)

## Temario
1. Del primer módulo:
   - Identificar los beneficios de la nube
   - Diferencias entre Opex y Capex
   - Describir el módelo basado en el consumo
   - IaaS,PaaS y SaaS 
   - Nube pública,privada e híbrida
   - Comparar los tres tipos de cloud
   - Describir la computación sin servidor
   - Definición de computación en la nube
2. Del segundo módulo: (Parten de 10 servicios general,de los cuales parten muchos más)
   - Uso de regiones y pares regionales
   - Uso de zonas de disponibilidad
   - Uso de los grupos de recursos
   - Beneficios de usar máquinas virtuales
   - Uso de contenedores
   - Uso de redes virtuales(VLAN)
   - Uso de Azure Marketplace
   - Uso de recursos en Azure
   - Uso de bases de datos de Azure
3. Del tercer módulo
   - IoT,HUB,IoT Central y Azure Sphere
   - Machine Learning,Cognitive Services
   - Synapse Analytics,HDInsight
   - Describir el uso de Azure Monitor
   - Uso de Azure Advisor
   - Uso de Azure Resource Manager
4. Del cuarto módulo:
   - Rasgos básicos de Azure Security Center
   - Uso de Key Vault
   - Uso de Azure Sentinel
   - Concepto de Seguridad en profundidad
   - Uso de grupos de seguridad en la red
   - Uso de Azure Firewall
5. Del quinto módulo:
   - Autenticación y Autorización
   - Azure Active Directory
   - Control de acceso basado en roles
6. Del sexto módulo:
   - Factores que modifican precio
   - Reducción de costos
   - Uso de calculadora de Azure
## Cómputo en la nube
`Son servicios de computación,virtuales,que se ofrecen en una red`  
Pilares:  
1. El cliente escoge todo  
2. Acceso desde cualquier sitio  
3. Elasticidad y flexibilidad  
4. Tiene un costo menor
5. Grandes niveles de seguridad
6. Servicios de mejor rendimiento   

### Máquinas virtuales (cómo servicio)
`Un software capaz de soportar un sistema operativo,dentro de otro sistema operativo`
- Máquinas virtuales de Sistema  
`Emula a un ordenador completo, tiene sus recursos como memoria RAM, disco duro virtual, etc.`
- Máquinas virtuales de proceso  
`Emula a un proceso en específico, como por ejemplo: Ejecutar una aplicación, ejecutar JVM`  
Características:
1. Como medida de seguridad
2. Para tener más dinamismo
3. Para comprobar múltiples sistemas

### Contenedores
`Son entornos donde se almacenan aplicaciones con sus bibliotecas`  
[Más información,aquí](https://www.netapp.com/es/devops-solutions/what-are-containers/)

### Serverless
`Es computación sin un servidor dedicado inicialmente. El proveedor de la nube ejecuta el código de la app,se cobra por los recursos consumidos al ejecutar esta.`  
Características:  
1. Cobro por tener el servicio activo (ejecutandose)
2. Actualización del servidor (automáticamente)
3. No se administra el escalamiento del servidor

### Infraestructura tradicional

`Es todo lo referente a lo físico o infraestructura física, a la cual se le da mantenimiento a todos sus componentes`
`Mantenimiento : Todo lo que se debe hacer para optimizar o reparar los sistemas de red, servidor, network, etc.`  
Ventajas:  
1. El personal tiene conocimiento sobre toda la infraestructura  
2. Es preferencia en cuestión de seguridad
3. Tienes todo el control en la parte física  

Desventajas:  
1. Cualquier error recae sobre el personal de mantenimiento
2. Si un sistema cae o falla,el personal deberá presentar para solucionar el problema

### Infraestructura como servicio
`Provee el fundamento y base de Cloud Computing, es decir la infraestructura física en la nube, ya virtualizada y administrable a través de internet`  
¿Qué proporciona? : 
1. Servidores y computadoras virtuales
2. Datacenter virtuales
3. Seguridad virtual
4. Capacidad de almacenamiento
5. Redes virtuales

### Plataforma como servicio
`Servicio que nos permite desarrollar sistemas y ejecutar sus propios programas y aplicaciones en distintos lenguajes`

### Software como servicio
`Provee aplicaciones para ser consumido por el usuario`

### Storage como servicio
`Provee de una infraestructura de almacenamiento`

### Network como servicio
`Conectividad de transporte de red.NaaS implica la optimización de las asignaciones de recursos al considerar los recursos informáticos y de red como un todo unificado`

### Comunication como servicio
`Comunicaciones unificadas son una categoría de mecanismos de entrega "como servicio" para las comunicaciones empresariales`

### CapEx y OpEx
Gastos en capital (CapEx)
`Es comprar activos con antelación,para implementarlos dentro de la empresa(O negocio)`
Gastos operativos (OpEx)
`Son gastos operativos de la empresa,y que se pagan luego de usarlos`