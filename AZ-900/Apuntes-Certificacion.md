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

## Formas de implementar la nube

### Nube pública
Es una infraestructura para todos. Cualquiera puede comprarla a un proveedor de nube.  
Beneficios:
- Fácil configuración e implementación
- Escalabilidad
- Pago por uso
- Reduce gastos
### Nube privada
Servicio privado que se ofrece a ciertos usuarios y se hace en un propio centro de datos.
### Nube híbrida
Es la mezcla de los beneficios de la nube pública y privada como son el rendimiento y desempeño,no dependencia de ambas para funcionar, mejor estructura y la separación de datos y obligaciones.

## Azure y sus servicios
¿Qué es Azure? : `Microsoft Azure son servicios de cloud computing, ofrecidos por Microsoft`
Características:
- Almacenamiento
- Infraestructura
- Interconexión
- Procesabilidad
- Administración
- CDN
### Servicios de cómputo
1. Azure Virtual Machines : Máquinas virtuales de sistemas operativos Linux o Windows.
2. Azure Virtual Machines Scale Sets : Son servicios para poder escalar las máquinas virtuales.
3. Azure Services Fabric : Subplataforma para sistemas distribuidos en redes. (Subredes)
4. Azure functions : Se basa en eventos y tiene como principal característica el uso de Serverless.
5. Azure Batch : Sirve para tener rendimientos altos en aplicaciones que lo requieran.
6. Azure Kubernetes Service : Su función es agrupar las aplicaciones en clústers y con contenedores.
7. Azure container instances : Implementar contenedores para poder ejecutar las web app

### Servicios de redes
1. Azure Virtual Network : Sirve para crear redes virtuales dentro de un servidor de Cloud.
2. Azure Load Balancer : Maneja el tráfico y ancho de banda de entrada y salida de la red.
3. Azure Application Gateway : Optimiza el tiempo dentro de las granjas de servidores
4. Azure content delivery network : Proporciona cierto contenido para el ancho de banda.
5. Azure Traffic Manager : Sirve para fijar una distribución de tráico dentro de toda la red.
6. Azure Network Watcher : Su función es supervisar y diagnosticar problemas dentro de la red.
7. Azure VPN Gateway : Implementa las VPN para hacer conexiones remotas.
8. Azure DNS : Asigna DNS y dominios para las aplicaciones web dentro de Azure.
9. Azure Express Route : Crea un túnel de conexión segura hacia Azure.
10. Azure DDoS Protection : Protege de todos los ataques de DDoS que puede sufrir la red.
11. Azure Firewall : Activa un firewall para la protección de la red.
12. Azure Virtual WAN : Crea una Red WAN para el acceso a Internet o alguna otra red.

### Servicios de almacenamiento
1. Azure Table Storage : Almacenamiento para NoSQL
2. Azure File Storage : Sirve para compartir archivos en red compartida.
3. Azure Queue Storage : Su función es la entrega de mensajes (Cola y entrega).
4. Azure Blob Storage : Proporciona almacenamiento para archivos grandes.

### Servicios de bases de datos
1. Azure Cosmos DB : Base de datos, que permite incorporar NoSQL
2. Azure SQL Database : Base de datos, que solo admite modelos relacionales (con motor SQL Server)
3. Azure Database for MySQL : Base de datos, que toma como base al gestor MySQL
4. Azure Database for PostgreSQL : Base de datos, que toma como base al gestor PostgreSQL
5. Azure Database for MariaDB : Base de datos, que toma como base al gestor MariaDB
6. SQL Server on Virtual Machines : Dirección Host de aplicaciones empresariales de SQL
7. Azure SQL Data Warehouse : Colección de datos también llamado almacen de datos
8. Azure Database Migration Service : Migrar los servicios de una base de datos hacia otra
9. Azure Cache for Redis : Caché de datos estáticos de una base de datos

### Servicios Web
1. Azure App Services : Creación de app que se basan en cloud
2. Azure API Management : Crea API´s para las aplicaciones que están en Cloud
3. Azure Notification Hubs : Cuando se desarrollan Apps en Cloud, siempre debe haber un backend. Sirve para enviar notificaciones desde backend
4. Azure cognitive search : Administra las búsquedas realizadas dentro de la nube
5. Azure SignalR Service : Implementa un monitoreo en tiempo real sobre las aplicaciones web
6. Web Apps features of Azure App Service : Sirve para alojar una app web de una escala muy alta

### Servicios de IoT y Big Data
1. IoT Edge : Son módelos de datos ya establecidos , para realizar análisis
2. IoT Central : Es un SaaS. Facilita la conexión entre dispositovs IoT 
3. Azure IoT Hub : Se encarga de distribuir mensajería entre dispositivos IoT
4. Azure SQL Data Warehouse : Su función es la de analizar datos a profundidad y a gran escala
5. Azure HDInsight : Permite procesar una cantidad grande de datos, organizados en Clústers
6. Azure Databricks : Permite que el análisis de datos pueda ser colaborativo
   
### Servicios de Inteligencia Artificial y DevOps
1. Azure Machine Learning Service : Implementar modelos de aprendizaje automático
2. Azure Machine Learning Studio : Crea algoritmos de aprendizaje automátizado
3. Azure DevOps : Facilita la colaboración conjunta de desarrolladores para un proyecto
4. Azure DevTest Labs : Crea entornos Linux o Windows, que permiten probar las aplicaciones web

### Servicios cognitivos
1. Vision : Procesa imágenes y vídeos con ayuda de inteligencia artificial
2. Speech : Permite convertir audio en texto
3. Big Search : Posibilita implementar una API para usarla como buscador
4. Natural Language Processing : Procesa lenguaje natural y común, pero con scripts automatizados

### Grupo de recursos
Contenedor lógico, que contiene los recursos o servicios implementados en Azure.  
Facilita la administración y eliminación de recursos en conjunto.
### Azure resource manager
Proporciona una capa de administración, que nos permite modificación de recursos,características de autenticación y demás. Editas recursos ya existentes.
### Etiquetas de servicios
Son nombres y valores de datos para asociar detalles entre nuestros recursos. Un recurso puede tener hasta 50 etiquetas

## Servicios de almacenamiento de datos y recursos en Azure
Tipos de almacenamiento:
- Cloud
- On-Premises (Local)  
Características

\  |On-Premises|Azure
---|---|---
Costos|Requiere hardware dedicado que requiere manejar la demanda máxima|Ofrece almacenamiento de pago y escalable listo para cumplir funciones de demanda
Confiabilidad|Requiere balanceo de carga y recuperación ante desastres y copia de seguridad|Ya proporciona estos servicios de forma integrada

**Ventajas de usar Azure para almacenar tus datos :**  
- Replicación : Copias de tus datos en cualquier parte del mundo
- Cifrado : Cifrado en las comunicaciones,verifica los accesos y bloquearlos
- Compatibilidad con análisis de base de datos
- Backups automátizados : Permite programar backups y nos proporciona recuperación de desastres
- Almacenamiento en discos virtuales : Almacenar hasta 32 TB en discos virtuales

**Servicios de Azure para manejar el almacenamiento :**
- Azure Queues : Permite almacenar una gran cantidad de datos
- Database SQL : Ofrece un servicio de SQL con última versión actualizada, dandote la infraestructura
- Azure Disk : Montar máquinas virtuales, según nuestras necesidades
- Azure data lake : Nos permite el procesamiento de datos sin importar su tamaño,forma o velocidad de transferencia
  
## Infraestructura de Azure 
### Distribución de centro de datos y regiones en Azure
Existen muchas: Canada East,Canada Central,US Gov lowa,Central US,North Central US,West US 2, West US, US Gov Arizona,US DoD East,East US,East US 2,US Gov Virginia,West Central US,US Gov Texas,US DoD Central,South Central US,Brazil South,UK South,North,Europe,West Europe,UK West,Germany Northeast,Germany Central,West India,Central India,South India,China North,China East,East Asia,Southeast Asia,Korea Central,Korea South,Japan East,Japan West,Australia East,Australia Southeast.  
Pronto : France Central,France South, South Africa North, South Africa West, Australia Central, Australia Central 2
### Geografía en servicios de Azure
Ubicación donde se encuentran tus datos. Todos tienen :
- Tolerancia ante fallos
- Cumplimiento de datos y de residencia
- Cuidar el mercado de regiones
### Zonas de disponibilidad en Azure
Centro físico que se encuentra dentro de una región
### Regiones pares
Centros físicos alejados pero que se encuentran dentro de una misma región.

## Concepto de Redes de Azure
### Red Virtual Azure 
Es una red virtual aislada y de alta seguridad, que nos permite la ejecución de máquinas virtuales y aplicaciones