# Apuntes - Certificacion AZ-900
<!-- vscode-markdown-toc -->
* 1. [Contenido](#Contenido)
* 2. [Introducción](#Introduccin)
* 3. [Temario](#Temario)
* 4. [Cómputo en la nube](#Cmputoenlanube)
	* 4.1. [Máquinas virtuales (cómo servicio)](#Mquinasvirtualescmoservicio)
	* 4.2. [Contenedores](#Contenedores)
	* 4.3. [Serverless](#Serverless)
	* 4.4. [Infraestructura tradicional](#Infraestructuratradicional)
	* 4.5. [Infraestructura como servicio](#Infraestructuracomoservicio)
	* 4.6. [Plataforma como servicio](#Plataformacomoservicio)
	* 4.7. [Software como servicio](#Softwarecomoservicio)
	* 4.8. [Storage como servicio](#Storagecomoservicio)
	* 4.9. [Network como servicio](#Networkcomoservicio)
	* 4.10. [Comunication como servicio](#Comunicationcomoservicio)
	* 4.11. [CapEx y OpEx](#CapExyOpEx)
* 5. [Formas de implementar la nube](#Formasdeimplementarlanube)
	* 5.1. [Nube pública](#Nubepblica)
	* 5.2. [Nube privada](#Nubeprivada)
	* 5.3. [Nube híbrida](#Nubehbrida)
* 6. [Azure y sus servicios](#Azureysusservicios)
	* 6.1. [Servicios de cómputo](#Serviciosdecmputo)
	* 6.2. [Servicios de redes](#Serviciosderedes)
	* 6.3. [Servicios de almacenamiento](#Serviciosdealmacenamiento)
	* 6.4. [Servicios de bases de datos](#Serviciosdebasesdedatos)
	* 6.5. [Servicios Web](#ServiciosWeb)
	* 6.6. [Servicios de IoT y Big Data](#ServiciosdeIoTyBigData)
	* 6.7. [Servicios de Inteligencia Artificial y DevOps](#ServiciosdeInteligenciaArtificialyDevOps)
	* 6.8. [Servicios cognitivos](#Servicioscognitivos)
	* 6.9. [Grupo de recursos](#Grupoderecursos)
	* 6.10. [Azure resource manager](#Azureresourcemanager)
	* 6.11. [Etiquetas de servicios](#Etiquetasdeservicios)
* 7. [Servicios de almacenamiento de datos y recursos en Azure](#ServiciosdealmacenamientodedatosyrecursosenAzure)
* 8. [Infraestructura de Azure](#InfraestructuradeAzure)
	* 8.1. [Distribución de centro de datos y regiones en Azure](#DistribucindecentrodedatosyregionesenAzure)
	* 8.2. [Geografía en servicios de Azure](#GeografaenserviciosdeAzure)
	* 8.3. [Zonas de disponibilidad en Azure](#ZonasdedisponibilidadenAzure)
	* 8.4. [Regiones pares](#Regionespares)
* 9. [Concepto de Redes de Azure](#ConceptodeRedesdeAzure)
	* 9.1. [Red Virtual Azure](#RedVirtualAzure)
	* 9.2. [Disponibilidad y resiliencia de las redes en Azure](#DisponibilidadyresilienciadelasredesenAzure)
	* 9.3. [Azure DNS](#AzureDNS)
	* 9.4. [Equilibrador de carga](#Equilibradordecarga)
	* 9.5. [CDN de Azure](#CDNdeAzure)
* 10. [Seguridad en redes de Azure](#SeguridadenredesdeAzure)
	* 10.1. [Grupos de seguridad en redes de Azure](#GruposdeseguridadenredesdeAzure)
	* 10.2. [Gestor de tráfico en Azure](#GestordetrficoenAzure)
	* 10.3. [Traffic Manager vs Load Balancer](#TrafficManagervsLoadBalancer)
	* 10.4. [Azure Application Gateway](#AzureApplicationGateway)
	* 10.5. [Azure Front Door](#AzureFrontDoor)
* 11. [Seguridad en Azure](#SeguridadenAzure)
	* 11.1. [Responsabilidad compartida](#Responsabilidadcompartida)
	* 11.2. [Identidad de Azure](#IdentidaddeAzure)
	* 11.3. [Azure Security Center](#AzureSecurityCenter)
	* 11.4. [Cifrado en Azure](#CifradoenAzure)
	* 11.5. [Certificados](#Certificados)
	* 11.6. [Protección de información y Advance Threat Protection](#ProteccindeinformacinyAdvanceThreatProtection)
* 12. [Políticas de Azure,Seguridad y Gobernanza de Azure](#PolticasdeAzureSeguridadyGobernanzadeAzure)
	* 12.1. [Declaración de privacidad](#Declaracindeprivacidad)
	* 12.2. [Microsoft Trust Center](#MicrosoftTrustCenter)
	* 12.3. [Azure Policy](#AzurePolicy)
	* 12.4. [Gobernanza de suscripción](#Gobernanzadesuscripcin)
	* 12.5. [Azure Blueprint](#AzureBlueprint)
	* 12.6. [Compliance Manager](#ComplianceManager)
	* 12.7. [Compliance Manager y Service Healt](#ComplianceManageryServiceHealt)
* 13. [Costos en Azure](#CostosenAzure)
	* 13.1. [Factores de costos](#Factoresdecostos)
	* 13.2. [Azure Advisor](#AzureAdvisor)
	* 13.3. [Ahorro de costos](#Ahorrodecostos)
* 14. [Acuerdos de nivel de servicio en Azure](#AcuerdosdeniveldeservicioenAzure)
	* 14.1. [SLA de Azure](#SLAdeAzure)
	* 14.2. [SLA de aplicación](#SLAdeaplicacin)
* 15. [Preguntas](#Preguntas)

<!-- vscode-markdown-toc-config
	numbering=true
	autoSave=true
	/vscode-markdown-toc-config -->
<!-- /vscode-markdown-toc --># Microsoft Azure Certified AZ-900 Fundamentals
##  1. <a name='Contenido'></a>Contenido
- [Introducción](#temario)
- [Temario](#temario)
- [Cómputo en la Nube](#cómputo-en-la-nube)
- [Formas de implementar la nube](#formas-de-implementar-la-nube)
  
##  2. <a name='Introduccin'></a>Introducción 
El examen consta de 6 módulos importantes
1. Describir los conceptos de la nube
2. Describir los servicios centrales de Azure
3. Describir las soluciones y las herramientas de administración de Azure
4. Describir las características principales de seguridad y seguridad en la red
5. Describir las características de gobernanza, identidad, privacidad y cumplimiento
6. Describir la administración de costos de Azure y los SLA(Acuerdo de nivel de servicio)
##  3. <a name='Temario'></a>Temario
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
##  4. <a name='Cmputoenlanube'></a>Cómputo en la nube
`Son servicios de computación,virtuales,que se ofrecen en una red`  
Pilares:  
1. El cliente escoge todo  
2. Acceso desde cualquier sitio  
3. Elasticidad y flexibilidad  
4. Tiene un costo menor
5. Grandes niveles de seguridad
6. Servicios de mejor rendimiento   

###  4.1. <a name='Mquinasvirtualescmoservicio'></a>Máquinas virtuales (cómo servicio)
`Un software capaz de soportar un sistema operativo,dentro de otro sistema operativo`
- Máquinas virtuales de Sistema  
`Emula a un ordenador completo, tiene sus recursos como memoria RAM, disco duro virtual, etc.`
- Máquinas virtuales de proceso  
`Emula a un proceso en específico, como por ejemplo: Ejecutar una aplicación, ejecutar JVM`  
Características:
1. Como medida de seguridad
2. Para tener más dinamismo
3. Para comprobar múltiples sistemas

###  4.2. <a name='Contenedores'></a>Contenedores
`Son entornos donde se almacenan aplicaciones con sus bibliotecas`  
[Más información,aquí](https://www.netapp.com/es/devops-solutions/what-are-containers/)

###  4.3. <a name='Serverless'></a>Serverless
`Es computación sin un servidor dedicado inicialmente. El proveedor de la nube ejecuta el código de la app,se cobra por los recursos consumidos al ejecutar esta.`  
Características:  
1. Cobro por tener el servicio activo (ejecutandose)
2. Actualización del servidor (automáticamente)
3. No se administra el escalamiento del servidor

###  4.4. <a name='Infraestructuratradicional'></a>Infraestructura tradicional

`Es todo lo referente a lo físico o infraestructura física, a la cual se le da mantenimiento a todos sus componentes`
`Mantenimiento : Todo lo que se debe hacer para optimizar o reparar los sistemas de red, servidor, network, etc.`  
Ventajas:  
1. El personal tiene conocimiento sobre toda la infraestructura  
2. Es preferencia en cuestión de seguridad
3. Tienes todo el control en la parte física  

Desventajas:  
1. Cualquier error recae sobre el personal de mantenimiento
2. Si un sistema cae o falla,el personal deberá presentar para solucionar el problema

###  4.5. <a name='Infraestructuracomoservicio'></a>Infraestructura como servicio
`Provee el fundamento y base de Cloud Computing, es decir la infraestructura física en la nube, ya virtualizada y administrable a través de internet`  
¿Qué proporciona? : 
1. Servidores y computadoras virtuales
2. Datacenter virtuales
3. Seguridad virtual
4. Capacidad de almacenamiento
5. Redes virtuales

###  4.6. <a name='Plataformacomoservicio'></a>Plataforma como servicio
`Servicio que nos permite desarrollar sistemas y ejecutar sus propios programas y aplicaciones en distintos lenguajes`

###  4.7. <a name='Softwarecomoservicio'></a>Software como servicio
`Provee aplicaciones para ser consumido por el usuario`

###  4.8. <a name='Storagecomoservicio'></a>Storage como servicio
`Provee de una infraestructura de almacenamiento`

###  4.9. <a name='Networkcomoservicio'></a>Network como servicio
`Conectividad de transporte de red.NaaS implica la optimización de las asignaciones de recursos al considerar los recursos informáticos y de red como un todo unificado`

###  4.10. <a name='Comunicationcomoservicio'></a>Comunication como servicio
`Comunicaciones unificadas son una categoría de mecanismos de entrega "como servicio" para las comunicaciones empresariales`

###  4.11. <a name='CapExyOpEx'></a>CapEx y OpEx
Gastos en capital (CapEx)
`Es comprar activos con antelación,para implementarlos dentro de la empresa(O negocio)`
Gastos operativos (OpEx)
`Son gastos operativos de la empresa,y que se pagan luego de usarlos`
##  5. <a name='Formasdeimplementarlanube'></a>Formas de implementar la nube

###  5.1. <a name='Nubepblica'></a>Nube pública
Es una infraestructura para todos. Cualquiera puede comprarla a un proveedor de nube.  
Beneficios:
- Fácil configuración e implementación
- Escalabilidad
- Pago por uso
- Reduce gastos
###  5.2. <a name='Nubeprivada'></a>Nube privada
Servicio privado que se ofrece a ciertos usuarios y se hace en un propio centro de datos.
###  5.3. <a name='Nubehbrida'></a>Nube híbrida
Es la mezcla de los beneficios de la nube pública y privada como son el rendimiento y desempeño,no dependencia de ambas para funcionar, mejor estructura y la separación de datos y obligaciones.
##  6. <a name='Azureysusservicios'></a>Azure y sus servicios
¿Qué es Azure? : `Microsoft Azure son servicios de cloud computing, ofrecidos por Microsoft`
Características:
- Almacenamiento
- Infraestructura
- Interconexión
- Procesabilidad
- Administración
- CDN
###  6.1. <a name='Serviciosdecmputo'></a>Servicios de cómputo
1. Azure Virtual Machines : Máquinas virtuales de sistemas operativos Linux o Windows.
2. Azure Virtual Machines Scale Sets : Son servicios para poder escalar las máquinas virtuales.
3. Azure Services Fabric : Subplataforma para sistemas distribuidos en redes. (Subredes)
4. Azure functions : Se basa en eventos y tiene como principal característica el uso de Serverless.
5. Azure Batch : Sirve para tener rendimientos altos en aplicaciones que lo requieran.
6. Azure Kubernetes Service : Su función es agrupar las aplicaciones en clústers y con contenedores.
7. Azure container instances : Implementar contenedores para poder ejecutar las web app

###  6.2. <a name='Serviciosderedes'></a>Servicios de redes
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

###  6.3. <a name='Serviciosdealmacenamiento'></a>Servicios de almacenamiento
1. Azure Table Storage : Almacenamiento para NoSQL
2. Azure File Storage : Sirve para compartir archivos en red compartida.
3. Azure Queue Storage : Su función es la entrega de mensajes (Cola y entrega).
4. Azure Blob Storage : Proporciona almacenamiento para archivos grandes.

###  6.4. <a name='Serviciosdebasesdedatos'></a>Servicios de bases de datos
1. Azure Cosmos DB : Base de datos, que permite incorporar NoSQL
2. Azure SQL Database : Base de datos, que solo admite modelos relacionales (con motor SQL Server)
3. Azure Database for MySQL : Base de datos, que toma como base al gestor MySQL
4. Azure Database for PostgreSQL : Base de datos, que toma como base al gestor PostgreSQL
5. Azure Database for MariaDB : Base de datos, que toma como base al gestor MariaDB
6. SQL Server on Virtual Machines : Dirección Host de aplicaciones empresariales de SQL
7. Azure SQL Data Warehouse : Colección de datos también llamado almacen de datos
8. Azure Database Migration Service : Migrar los servicios de una base de datos hacia otra
9. Azure Cache for Redis : Caché de datos estáticos de una base de datos

###  6.5. <a name='ServiciosWeb'></a>Servicios Web
1. Azure App Services : Creación de app que se basan en cloud
2. Azure API Management : Crea API´s para las aplicaciones que están en Cloud
3. Azure Notification Hubs : Cuando se desarrollan Apps en Cloud, siempre debe haber un backend. Sirve para enviar notificaciones desde backend
4. Azure cognitive search : Administra las búsquedas realizadas dentro de la nube
5. Azure SignalR Service : Implementa un monitoreo en tiempo real sobre las aplicaciones web
6. Web Apps features of Azure App Service : Sirve para alojar una app web de una escala muy alta

###  6.6. <a name='ServiciosdeIoTyBigData'></a>Servicios de IoT y Big Data
1. IoT Edge : Son módelos de datos ya establecidos , para realizar análisis
2. IoT Central : Es un SaaS. Facilita la conexión entre dispositovs IoT 
3. Azure IoT Hub : Se encarga de distribuir mensajería entre dispositivos IoT
4. Azure SQL Data Warehouse : Su función es la de analizar datos a profundidad y a gran escala
5. Azure HDInsight : Permite procesar una cantidad grande de datos, organizados en Clústers
6. Azure Databricks : Permite que el análisis de datos pueda ser colaborativo
   
###  6.7. <a name='ServiciosdeInteligenciaArtificialyDevOps'></a>Servicios de Inteligencia Artificial y DevOps
1. Azure Machine Learning Service : Implementar modelos de aprendizaje automático
2. Azure Machine Learning Studio : Crea algoritmos de aprendizaje automátizado
3. Azure DevOps : Facilita la colaboración conjunta de desarrolladores para un proyecto
4. Azure DevTest Labs : Crea entornos Linux o Windows, que permiten probar las aplicaciones web

###  6.8. <a name='Servicioscognitivos'></a>Servicios cognitivos
1. Vision : Procesa imágenes y vídeos con ayuda de inteligencia artificial
2. Speech : Permite convertir audio en texto
3. Big Search : Posibilita implementar una API para usarla como buscador
4. Natural Language Processing : Procesa lenguaje natural y común, pero con scripts automatizados

###  6.9. <a name='Grupoderecursos'></a>Grupo de recursos
Contenedor lógico, que contiene los recursos o servicios implementados en Azure.  
Facilita la administración y eliminación de recursos en conjunto.
###  6.10. <a name='Azureresourcemanager'></a>Azure resource manager
Proporciona una capa de administración, que nos permite modificación de recursos,características de autenticación y demás. Editas recursos ya existentes.
###  6.11. <a name='Etiquetasdeservicios'></a>Etiquetas de servicios
Son nombres y valores de datos para asociar detalles entre nuestros recursos. Un recurso puede tener hasta 50 etiquetas
##  7. <a name='ServiciosdealmacenamientodedatosyrecursosenAzure'></a>Servicios de almacenamiento de datos y recursos en Azure
Tipos de almacenamiento:
- Cloud
- On-Premises (Local)  
Características

| \             | On-Premises                                                                   | Azure                                                                             |
| ------------- | ----------------------------------------------------------------------------- | --------------------------------------------------------------------------------- |
| Costos        | Requiere hardware dedicado que requiere manejar la demanda máxima             | Ofrece almacenamiento de pago y escalable listo para cumplir funciones de demanda |
| Confiabilidad | Requiere balanceo de carga y recuperación ante desastres y copia de seguridad | Ya proporciona estos servicios de forma integrada                                 |

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
##  8. <a name='InfraestructuradeAzure'></a>Infraestructura de Azure 
###  8.1. <a name='DistribucindecentrodedatosyregionesenAzure'></a>Distribución de centro de datos y regiones en Azure
Existen muchas: Canada East,Canada Central,US Gov lowa,Central US,North Central US,West US 2, West US, US Gov Arizona,US DoD East,East US,East US 2,US Gov Virginia,West Central US,US Gov Texas,US DoD Central,South Central US,Brazil South,UK South,North,Europe,West Europe,UK West,Germany Northeast,Germany Central,West India,Central India,South India,China North,China East,East Asia,Southeast Asia,Korea Central,Korea South,Japan East,Japan West,Australia East,Australia Southeast.  
Pronto : France Central,France South, South Africa North, South Africa West, Australia Central, Australia Central 2
###  8.2. <a name='GeografaenserviciosdeAzure'></a>Geografía en servicios de Azure
Ubicación donde se encuentran tus datos. Todos tienen :
- Tolerancia ante fallos
- Cumplimiento de datos y de residencia
- Cuidar el mercado de regiones
###  8.3. <a name='ZonasdedisponibilidadenAzure'></a>Zonas de disponibilidad en Azure
Centro físico que se encuentra dentro de una región
###  8.4. <a name='Regionespares'></a>Regiones pares
Centros físicos alejados pero que se encuentran dentro de una misma región.
##  9. <a name='ConceptodeRedesdeAzure'></a>Concepto de Redes de Azure
###  9.1. <a name='RedVirtualAzure'></a>Red Virtual Azure 
Es una red virtual aislada y de alta seguridad, que nos permite la ejecución de máquinas virtuales y aplicaciones.  
| Característica                  | Descripción                                                                                                                                   |
| ------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------- |
| Monitorear                      | La red de Azure nos permite monitorear toda la red y supervisarla.                                                                            |
| Comunicación                    | La red virtual nos permite difnir la forma en cómo se comunicarán internamente,al igual que cómo el usuario va a interactuar con el servicio. |
| Aislar                          | Aisla nuestra red y mantenerla de forma "privada" incluyendo componentes dentro de la nube.                                                   |
| Protección                      | Permite definir reglas de firewall, para mantener segura la red en sí.                                                                        |
| Segmentación de redes virtuales | Azure nos permite segmentar las redes virtuales, definiendo también así los accesos.                                                          |

###  9.2. <a name='DisponibilidadyresilienciadelasredesenAzure'></a>Disponibilidad y resiliencia de las redes en Azure
| Tipo           | Descripción                                                                |
| -------------- | -------------------------------------------------------------------------- |
| Disponibilidad | Tiempo por el cual el servicio estará en funcionamiento.                   |
| Resiliencia    | Proporciona mecanismos para recuperarse después que el sistema ha fallado. |

###  9.3. <a name='AzureDNS'></a>Azure DNS
DNS : `Sistema de dominio de red, es un sistema el cual nos permite ponerle nombres a las direcciones IP`.  
Azure DNS usa el mismo concepto de DNS,solo que aplicado al entorno de Azure, para una mejor optimización en la red.

###  9.4. <a name='Equilibradordecarga'></a>Equilibrador de carga
Es una balanceador de Azure que divide el tráfico de red de manera uniforme  y que sea de la misma región.
Nos ayuda a tener más disponibilidad y resiliencia.

###  9.5. <a name='CDNdeAzure'></a>CDN de Azure
Content Delivery Network, es una solución de red distribuida de servidores que entrega rápidamente contenido que requiere gran ancho de banda a los usuarios.  
Ayuda a ofrecer mejor rendimiento a los usuarios finales y una seguridad robusta.
##  10. <a name='SeguridadenredesdeAzure'></a>Seguridad en redes de Azure
###  10.1. <a name='GruposdeseguridadenredesdeAzure'></a>Grupos de seguridad en redes de Azure
El grupo de seguridad de red es aquel que monitorea el tráfico de red y define los accesos de este.  
Funciones:  
- Monitorear
- Supervisar
- Denegar accesos
- Permitir accesos
- Definir reglas de firewall

###  10.2. <a name='GestordetrficoenAzure'></a>Gestor de tráfico en Azure
(Azure Traffic Manager), es un gestor o balanceador de carga de tráfico basado en DNS que nos permite distribuir el tráfico de servicios en Azure.  
Nos ayuda a optimizar el tráfico de servicios entre regiones de Azure y crear resiliencia en todas las regiones de Azure.  
Características:
- Admite puntos de conexión externos a Azure
- Utiliza perfiles anidados
- Usa `failover` automático

###  10.3. <a name='TrafficManagervsLoadBalancer'></a>Traffic Manager vs Load Balancer

| \                | Azure Load Balancer       | Azure Traffic Manager                          |
| ---------------- | ------------------------- | ---------------------------------------------- |
| Balancear la red | En una sola región Azure  | En diferentes regiones Azure                   |
| Optimización     | En la entrega de paquetes | entrega de paquetes y reduce el ancho de banda |

###  10.4. <a name='AzureApplicationGateway'></a>Azure Application Gateway
Es un balanceador de carga de tráfico de red, que nos permite equilibrar el tráfico de las **aplicaciones web en Azure**.
Características:  
- Escalable
- Está integrado con otros servicios Azure
- Ofrece firewall de aplicaciones web
- Descarga SSL

###  10.5. <a name='AzureFrontDoor'></a>Azure Front Door
Es la puerta que permite la entrega rápida y segura de las aplicaciones web globales.
Características:  
- Aceleración de aplicaciones
- Balanceo de carga HTTP
- Protección de aplicaciones
- `failover` instántaneo  
Ventajas:  
- Aceleración HTTP
- Escalabilidad independiente
- Seguridad en linea
##  11. <a name='SeguridadenAzure'></a>Seguridad en Azure
###  11.1. <a name='Responsabilidadcompartida'></a>Responsabilidad compartida
Es la asignatura de responsabilidad entre proveedor y cliente.
###  11.2. <a name='IdentidaddeAzure'></a>Identidad de Azure
Son los diferentes accesos de los usuarios.
Cada usuario posee una identidad y cada identidad tiene acceso o autorización para entrar a ciertos servicios.  
**Autorización** : Al mencionar una autorizacións nos referismoa a que nivel de acceso tiene la persona.
**Azure Active Directory** : Es un servicio de identidad proporcionado por la nube y nos ofrece. 
- Admin App
- Autenticación
- SSO : `Procedimienot de autenticación,que habilita a un usuario determinado para acceder a varios sistemas con una sola instancia de identificación`  
Con Azure nos permite centralizar los controlres de seguridad,al igual,poder combinar el origen de datos para análisis de amenazas en tiempo real.
- Administración de dispositivo

**MFA** : Es un método multipruebas que da acceso al usuario, siempre y cuando haya pasado las pruebas impuestas.

###  11.3. <a name='AzureSecurityCenter'></a>Azure Security Center
Es un servicio que proporciona seguridad en tu entorno de Azure como en el entorno de tu red local.
Beneficios:  
- Guia a los ususarios para su configuración
- Aprendizaje automático
- Recomendaciones según tus configuraciones
- Identificar amenazas

###  11.4. <a name='CifradoenAzure'></a>Cifrado en Azure
Es un método de seguridad, donde se encripta la comunicación entre una conversación.
**Cifrado asimétrico** : Utiliza dos llaves para cifrar y descifrar datos. 
**Cifrado simétrico** : Solo necesita una lalve para poder cifrar y descifrar datos. 
**Datos en reposo** : Son datos que no se utilizan en la comunicación por el momento, es decir que no están pasando por un canal y están almacenados. 
**Datos en tránsito** : Son datos que se mueven de una localización a otra,la seguridad de estos pueden variar o usar varios métodos. 
**Azure Key Vault** : Servicio que nos permite proteger nuestra encriptación y podemos gestionar los diferentes accesos y llaves.

La encriptación de Azure nos ofrece :
- Servicio de encriptación de almacenamiento
- Encriptación de disco
- Encriptación de base de datos
- Secrets

###  11.5. <a name='Certificados'></a>Certificados
Son una medida de confianza adicional de protección para las personas que visitan y realizan transacciones en las páginas web, asegurando que su información está segura.

**Azure key vault con certificados** : En Azure Key Vault se puede crear y almacenar certificados,como una medida de mantenerlos en secreto, al igual que podemos importar certificados existentes y la renovación de estos, establecer políticas y notificaciones de eventos.

**Problemas con los certificados** : No todos están actualizados o protegan y exponen la seguridad de la página y comprometiendo la información de sus usuarios.

**¿Qué certificado ofrece Azure?** : Ofrece certificados X.509_V3, pueden ser auto firmados o firmados por una entidad de certificación de confianza.

**Certificado de administración** : Nos permite comunicarnos con la API de administración.

**Certificado de servicio** : Se utilizan para los servicios de la nube,permitiendo la comunicación segura hacía y desde el servicio.

###  11.6. <a name='ProteccindeinformacinyAdvanceThreatProtection'></a>Protección de información y Advance Threat Protection
**Azure information protection** es una solución basada en la nube que ayuda a clasificar y administrar elementos.  
Características:  
- Clasifica y protege documentos y correos mediante etiquetas
- Etiquetas pueden ser definidad de forma automática o manul
- Realización de seguimiento
- Tomar medidas correctivas

**Advance Threat Protection** es una solución de seguridad basada en la nube, la cual nos permite detectar y controlar amenazas avanzadas.
Características:  
- Detección y seguimiento de amenazas
- Detección de riesgos
- Análisis interno y externo

**Azure ATP** es una solución de seguridad, localizada en la nube que utiliza las señales de **Active Directory** local para inspeccionar,detectar y reconocer amenazas avanzadas.
##  12. <a name='PolticasdeAzureSeguridadyGobernanzadeAzure'></a>Políticas de Azure,Seguridad y Gobernanza de Azure
###  12.1. <a name='Declaracindeprivacidad'></a>Declaración de privacidad
Es la asignación al acceso de datos por parte de la organización . Proporciona una apertura y honestidad sobre como se trataran los datos personales del usuario.

###  12.2. <a name='MicrosoftTrustCenter'></a>Microsoft Trust Center
Sitio web que contiene la administración e implementación de medidas de seguridad en los servicios adquiridos.
Características:  
- Información especifica sobre los roles
- Búsqueda de documentos entre empresas
- Recomendaciones de recursos

**Portal de confianza de servicios** es un portal de transparencia donde se publican informes de auditoría e información relevante para los servicios de Microsoft.  
Permite descargar informes de auditoria,ver informes de auditoria externos a Microsoft, información del manejo de operaciones por Microsoft

###  12.3. <a name='AzurePolicy'></a>Azure Policy
Evalúa los recursos de Azure, comparando las propiedades de esos recursos con las reglas de negocio. Busca satisfacer 3 propositos : Cumplimiento y estándares, Aplicar políticas de escala,corregir y automatizar.

Términos: 
- *Policy* : Politicas a aplicar
- *Iniciative* : Coleccción de reglas
- *Assignment* : Alcance de aplicación

Ofrece: 
- Corregir los recursos existentes a escala
- Directiva como código Devops
- Alcance de exclusión
- etc.

**RBAC** es un nuevo sistema de autorización, que proporciona una administración de acceso detallada a los recursos de Azure.   
A diferencia de **Azure Policy**, **RBAC** se centra en las acciones que se pueden tomar en un solo ámbito y la denegación de accesos se da por defecto a menos que  nosotros lo implementemos explícitamente.

###  12.4. <a name='Gobernanzadesuscripcin'></a>Gobernanza de suscripción
Nos permite mantener un control de los accesos dentro de nuestro entorno Azure.  
Nos ayuda a administrar los accesos en un área específica, definiendolo como un control y administración de controles.

###  12.5. <a name='AzureBlueprint'></a>Azure Blueprint
Facilidad de medidas de seguridad,análisis y detección, adaptandose a nestándares de nuestra organización.
Nos permite la fácilidad de medidas de seugirdad,análisis y detección,adaptandose a estándares de neustra organización.  
Como se implmenta : 
- Creación de plantilla dedefinicióin
- Asegurar los recursos fundamentales
- Seguimiento de asignación  
Blueprint nos permite:
- Asignación de roles
- Asignación de políticas
- Implementación de plantillas
- etc

###  12.6. <a name='ComplianceManager'></a>Compliance Manager
Es una funcionalidad, la cual nos permite administrar lso requisitos de cumplimiento de nuestra organización
Características:  
1. Seguimiento de procesos
2. Inventario de riesgos
3. Mantenimiento de regulaciones y certificados

###  12.7. <a name='ComplianceManageryServiceHealt'></a>Compliance Manager y Service Healt
Es un panel de evaluación de riesgos dentro del portal de confianza.
- Recomendaciones de mejora
- Acciones recomendadas para mejorar el cumplimiento normativo
- Vista del panel para regulaciones
- Evaluación de riesgos continuos

**Azure Monitor** es un servicio que máximiza la disponibilidad y requerimientos de las aplicaciones ofreciendo una solución completa

Ofrece identifcación de problemas, recopilación de datos, registros de aplicación, ampliación de información, supervisión a nivel de sistemas operativos.

**Service Healt** es un servicio que notifica y ayuda a entender el impacto de los problemas.

Ofrece notificaciones sobre problemas, ayuda para planificaciones de mantenimiento, ayuda a comprender el impacto que pudiese tener en algún momento de caida
##  13. <a name='CostosenAzure'></a>Costos en Azure
###  13.1. <a name='Factoresdecostos'></a>Factores de costos
Costos que podría afectar al implementar los servicios de Azure
**Ubicación**, **Tipo de recurso**, **Tipos de suscripción**

###  13.2. <a name='AzureAdvisor'></a>Azure Advisor
Busca la manera de mejorar el ambiente en tus servicios

###  13.3. <a name='Ahorrodecostos'></a>Ahorro de costos
**Límite de gastos**: Azure contiene un límite de gasto, el cual se activa antes de que tu saldo llegue a cero para evitar cobros extra.  
**Ofertas**: Aprovechamiento de ofertas para minizar los costos, estas varían dependiendo la región.  
**Instancias reservadas** : Puedes usar instancias reservadas para minimizar el costo en un 70% dependiendo de tu máquina virtual.  
**Créditos de Azure** : Las suscripciones pueden contener lo que son beneficios de prueba, programación de funcionalidad de Azure y a cambio te proporcionan créditos.  
**Ubicaciones** : Usar suscripciones en regiones las cuales el costo de suscripción sea menor al que estas actualmente.  
**Detener y eliminar máquinas virtuales** : Detener máquinas virtuales cuando estas se ejecutan innecesariamente
****
##  14. <a name='AcuerdosdeniveldeservicioenAzure'></a>Acuerdos de nivel de servicio en Azure
Son los acuerdos los cuales contienen los términos específicos que definen los estándares que aplican a Azure. Existen acuerdo de nivel en productos y servicios
###  14.1. <a name='SLAdeAzure'></a>SLA de Azure 
Azure no define lo que es SLA para todos los servicios que proporciona.  
Características:  
1. Objetivos de rendimiento
2. Garantia de tiempo de actividad
3. Créditos de servicios  

###  14.2. <a name='SLAdeaplicacin'></a>SLA de aplicación
Al aplicar SLA como objetivo de rendimiento los cuales se adapten a nuestra aplicación de Azure.  
Permite la **disponibilidad**,**resiliencia**
##  15. <a name='Preguntas'></a>Preguntas
`Es el lugar donde se encuentra un centro de datos de Azure` : Región  
`Pide factores extra de autenticación, como preguntas predeterminadas` : Azure Multifactor