# **Microsoft Azure Fundamentals Course**
## **Temario**
- [**Microsoft Azure Fundamentals Course**](#microsoft-azure-fundamentals-course)
  - [**Temario**](#temario)
  - [**Cloud Computing y Conceptos clave**](#cloud-computing-y-conceptos-clave)
    - [**Cloud Computing**](#cloud-computing)
    - [**Conceptos clave**](#conceptos-clave)
  - [**Principios de economía de escala**](#principios-de-economía-de-escala)
  - [**CapEx vs OpEx y sus diferencias**](#capex-vs-opex-y-sus-diferencias)
  - [**Modelo basado en el consumo**](#modelo-basado-en-el-consumo)
  - [**IaaS vs PaaS vs SaaS Modelo de servicio cloud**](#iaas-vs-paas-vs-saas-modelo-de-servicio-cloud)
    - [**Matriz de responsabilidad**](#matriz-de-responsabilidad)
  - [**Modelos de implementación de nube pública, privada e híbrida**](#modelos-de-implementación-de-nube-pública-privada-e-híbrida)
    - [**Nube pública**](#nube-pública)
    - [**Nube privada**](#nube-privada)
    - [**Nube híbrida**](#nube-híbrida)
  - [**Geografía, Regiones y Zonas de disponibilidad**](#geografía-regiones-y-zonas-de-disponibilidad)
    - [**Data Center**](#data-center)
    - [**Región**](#región)
    - [**Zona de disponibilidad**](#zona-de-disponibilidad)
    - [**Pares de regiones**](#pares-de-regiones)
    - [**Geografías**](#geografías)
  - [**Recursos, grupos de recursos y administrador de recursos**](#recursos-grupos-de-recursos-y-administrador-de-recursos)
    - [**Recurso Azure**](#recurso-azure)
    - [**Grupo de recursos**](#grupo-de-recursos)
    - [**Administrador de recursos**](#administrador-de-recursos)
    - [**Información adicional**](#información-adicional)
  - [**Servicios de cómputo**](#servicios-de-cómputo)
    - [**Virtualización**](#virtualización)
    - [**Maquinas virtuales**](#maquinas-virtuales)
    - [**Conjuntos de escalado de máquinas virtuales**](#conjuntos-de-escalado-de-máquinas-virtuales)
    - [**Contenedores**](#contenedores)
    - [**Instancias de contenedores de Azure**](#instancias-de-contenedores-de-azure)
    - [**Servicio Azure Kubernetes (AKS)**](#servicio-azure-kubernetes-aks)
    - [**Servicio de aplicaciones(App Service)**](#servicio-de-aplicacionesapp-service)
    - [**Funciones de Azure (aplicaciones de funciones)**](#funciones-de-azure-aplicaciones-de-funciones)
    - [**Resumen**](#resumen)
  - [**Servicios de red**](#servicios-de-red)
    - [**Redes Azure (Azure Networking)**](#redes-azure-azure-networking)
    - [**Red virtual de Azure (Azure Virtual Network)**](#red-virtual-de-azure-azure-virtual-network)
    - [**Equilibrador de carga de Azure (Azure Load Balancer)**](#equilibrador-de-carga-de-azure-azure-load-balancer)
    - [**Puerta de enlace VPN**](#puerta-de-enlace-vpn)
    - [**Puerta de enlace de aplicaciones**](#puerta-de-enlace-de-aplicaciones)
    - [**Red de entrega de contenidos**](#red-de-entrega-de-contenidos)
  - [**Servicios de almacenamiento**](#servicios-de-almacenamiento)
    - [**Tipos de datos**](#tipos-de-datos)
    - [**Cuenta de almacenamiento**](#cuenta-de-almacenamiento)
    - [**Almacenamiento de blobs (Blob Storage)**](#almacenamiento-de-blobs-blob-storage)
    - [**Almacenamiento en cola (Queue Storage)**](#almacenamiento-en-cola-queue-storage)
    - [**Almacenamiento de tablas (Table Storage)**](#almacenamiento-de-tablas-table-storage)
    - [**Almacenamiento de archivos (File Storage)**](#almacenamiento-de-archivos-file-storage)
    - [**Almacenamiento de disco (Disk Storage)**](#almacenamiento-de-disco-disk-storage)
  - [**Servicios de bases de datos**](#servicios-de-bases-de-datos)
    - [**Tipos de datos en las BD**](#tipos-de-datos-en-las-bd)
    - [**Cosmos DB**](#cosmos-db)
    - [**SQL Database**](#sql-database)
    - [**Azure SQL product family**](#azure-sql-product-family)
  - [**Azure Marketplace**](#azure-marketplace)
  - [**Servicios IoT**](#servicios-iot)
    - [**Azure IoT Hub**](#azure-iot-hub)
    - [**Azure IoT Central**](#azure-iot-central)
    - [**Azure Sphere**](#azure-sphere)
  - [**Servicios Big Data & Analytics**](#servicios-big-data--analytics)
    - [**Azure Synapse Analytics**](#azure-synapse-analytics)
    - [**Azure HDInsight**](#azure-hdinsight)
    - [**Azure Databricks**](#azure-databricks)
  - [**Servicios de IA**](#servicios-de-ia)
    - [**Azure Machine Learning**](#azure-machine-learning)
  - [**Servicios serverless computing**](#servicios-serverless-computing)
    - [**Azure Functions**](#azure-functions)
    - [**Azure Logic Apps**](#azure-logic-apps)
    - [**Azure Event Grid**](#azure-event-grid)
  - [**Soluciones DevOps**](#soluciones-devops)
    - [**Azure DevOps**](#azure-devops)
    - [**Azure DevTest Labs**](#azure-devtest-labs)

## **Cloud Computing y Conceptos clave**
### **Cloud Computing**
Modelo de prestación de servicios a través de internet (nube). Esto incluye pero no se limita a
- **Compute power** es decir, servidores como Windows, Linux, entornos de alojamiento, etc.
- **Storage** como archivos y/o bases de datos
- **Networking** en azure pero también fuera cuando se conecta a la red de su empresa
- **Analytics** servicios de visualización y datos de telemetría  
<img src="Images/Cloud-Computing.png" alt="Cloud-Computing" width="300"/>

### **Conceptos clave**
- **Scalability** es la capacidad de escalar, así que asigna y desasigna recursos en cualquier momento.  
<img src="Images/Scalability.png" alt="Scalability" width="300"/>

- **Elasticity** es la capacidad de escalar dinámicamente.  
<img src="Images/Elasticity.png" alt="Elasticity" width="300"/>

- **Agility** es la capacidad de reaccionar rápido (escala rápidamente).  
<img src="Images/Agility.png" alt="Agility" width="300"/>

- **Fault tolerance** es la capacidad de mantener el tiempo de actividad del sistema mientras ocurren fallas físicas y de componentes de servicio.  
<img src="Images/Fault-Tolerance.png" alt="Fault-Tolerance" width="300"/>

- **Disaster Recovery** es el proceso y principio de diseño que permite que un sistema se recupere de desastres naturales o inducidos por el hombre.  
<img src="Images/Disaster-Recovery.png" alt="Disaster-Recovery" width="300"/> 

- **High Availability** es el nivel acordado de tiempo de actividad operativa para el sistema. Es un cálculo simple del tiempo de actividad del sistema frente a toda la vida útil del sistema.  
`disponibilidad = tiempo de actividad/(tiempo de actividad + tiempo de inactividad)`  
<img src="Images/High-Availability.png" alt="High-Availability" width="300"/>  

## **Principios de economía de escala**
El principio de economías de escala establece que a medida que las empresas crecen, se vuelven más efectivas en la gestión de operaciones compartidas. Ya sea recursos humanos y contratación, impuestos, contabilidad, operaciones internas, marketing, grandes compras a través de contratos que significan mejores descuentos, etc.  
Por eso,las empresas pueden ahorrar/ganar más, lo que a cambio les permite reducir el costo de sus servicios para sus clientes. Esto se llama **'precio por unidad'**.  
No es posible ir a 0 porque, al final, se debe ejecutar alguna infraestructura subyacente para proporcionar los servicios. Pero cuanto mayor sea la escala, más beneficios se pueden transferir a los clientes.  
De hecho, en la escala actual, Microsoft ya puede ofrecer múltiples servicios de forma gratuita debido a lo pequeña que es una fracción del costo para ellos.  
<div>
    <img src="Images/Economies-of-scale.png" alt="Economies-of-scale" width="300"/>  
    <img src="Images/Economies-of-scale-2.png" alt="Economies-of-scale-2" width="300"/>  
</div> 

## **CapEx vs OpEx y sus diferencias**
Diferencias entre gastos de capital(CapEx) y gastos operativos(OpEx)

/  |Gastos de capital|Gastos operacionales
---|---|---
Costo inicial|Significativo|Ninguno
Costo continuo|Bajo|Basado en el uso
Deducción fiscal|Tiempo extraordinario|Mismo año
Terminación anticipada|No|En cualquier momento
Mantenimiento|Significativo|Bajo
Valor en el tiempo|Disminuyen|Sin cambio
<div>
<img src="Images/CapEx.png" alt="CapEx" title="CapEx" width="300"/> 
<img src="Images/OpEx.png" alt="OpEx" title="OpEx" width="300"/> 
</div>  

Pregunta: `Having your own datacenter infraesutrcture has a big ______ cost associated`.  
Respuesta: `Initial`.  

## **Modelo basado en el consumo**
El modelo basado en el consumo es un modelo de precios que se utiliza en la nube para que a los clientes solo se les cobre en función de su uso de recursos.  
Este modelo se caracteriza por  

- **Sin costo inicial asociado**
- **No se desperdician recursos** como tal, *no se incurre en cargos por recursos no utilizados*. No utilizado en este caso es diferente por servicio. Por ejemplo, Se considera que se usa el almacenamiento de blobs que almacena cualquier dato, ya que consume el espacio de almacenamiento. Las máquinas virtuales que se ejecutan consumen CPU, memoria y otros recursos incluso si no hay tráfico. Por lo tanto, se consideran utilizados y generarán cargos.
- **Paga por lo que necesitas**
- **Deja de pagar cuando no lo haces**  
**El consumo** es la métrica virtual que se usa para calcular cuánto se usó cada recurso (servicio) en Azure. Cada servicio tiene muchas métricas más pequeñas que rastrean su consumo para ofrecer el mejor modelo de precios posible. Esas métricas se rastrean en un nivel muy granular.  
<img src="Images/Consumption-based-model.png" alt="CapEx" title="CapEx" width="300"/> 

[Consumption based Model - AZ-900 - Chapter Demo](https://youtu.be/NdqncsMtryY?list=PLGjZwEtPN7j-Q59JYso3L4_yoCjj2syrM) 

## **IaaS vs PaaS vs SaaS Modelo de servicio cloud**
Como servicio significa qué capa en particular administrará y todas las capas por encima.

- La capa de **Software** consiste en la aplicación (código y conjunto de la aplicación) y los datos de la aplicación. 
- La capa de **Platform** significa todo el software de soporte y el sistema oeprativo necesarios para alojar la aplicación.
- La capa de **Infraestructure** consta de hardware, la infraestructura y la virtualización necesarias para alojar la plataforma.

<img src="Images/Traditional.png" alt="Traditional" width="300"/> 

### **Matriz de responsabilidad**
Como tal, la siguiente tabla representa las responsabilidades.  
Layer(Capa)     |On-Premises|IaaS          |PaaS           |SaaS
---             |---       |---           |---            |---
Application     |Tú        |Tú           |Tú            |Cloud provider
Data            |Tú        |Tú           |Tú            |Cloud provider
Runtime         |Tú        |Tú           |Cloud provider |Cloud provider
Middleware      |Tú        |Tú           |Cloud provider |Cloud provider
Operating System|Tú        |Tú           |Cloud provider |Cloud provider
Virtualization  |Tú        |Cloud provider|Cloud provider |Cloud provider
Servers         |Tú        |Cloud provider|Cloud provider |Cloud provider
Networking      |Tú        |Cloud provider|Cloud provider |Cloud provider
Storage         |Tú        |Cloud provider|Cloud provider |Cloud provider

\  |Casos de Uso| Servicios de Azure
---|---|---
IaaS|<ul><li>Migración de cargas de trabajo</li><li>Test y Desarrollo</li><li>Almacenamiento</li><li>Backups y Recovery</li></ul>|<ul><li>Virtual Machine</li><li>Virtual Network</li><li>Managed Disk</li></ul>
PaaS|<ul><li>Development framework</li><li>Analytics & Business intelligence</li></ul>|<ul><li>SQL</li><li>App Service</li><li>Logic Apps</li><li>Function Apps</li></ul>
SaaS|<ul><li>Compra de aplicaciones shell</li></ul>|<ul><li>One Drive</li><li>Outlook</li><li>Skype</li></ul>

**NOTA** : Si instala SQL Server en una máquina virtual manualmente o al usar una imagen lista para usar, sigue siendo una máquina virtual. Eso significa que los clientes aún necesitan administrar todos
los aspectos de la plataforma. Esto incluye el sistema operativo,configuraciones, parches, middleware, configuraciones de tiempo de ejecución de SQL Server, etc. Como tal, sigue siendo una infraestructura como servicio.  
Azure tiene una opción para Azure SQL Server en máquina virtual donde todas las actualizaciones/copias de seguridad están automatizadas pero incluso Microsoft en su sitio web considera esta opción como IaaS,pero la línea es muy delgada aquí.

## **Modelos de implementación de nube pública, privada e híbrida**
El modelo de implementación en la nube es una separación simple que describe dónde se implementan los recursos de la empresa. Siempre que sea en un entorno de proveedor de nube pública o en un centro de datos privado.
### **Nube pública**
✅ Cloud Provider  ✖  Own Datacenter    
**Caracteristicas claves**
- Todo se ejecuta en el hardware del proveedor de la nube
- Sin hardware local
- Algunos servicios comparten hardware con otros clientes 

<table>
  <tr>
    <th>Ventajas</th>
    <th>Desventajas</th>
  </tr>
  <tr>
    <td><ul><li>Sin CapEx</li><li>Alta disponibilidad</li><li>Agilidad</li><li>Precios por pago de uso</li><li>Sin mantenimiento de hardware</li><li>No se requieren habilidades técnicas profundas</li></ul></td>
    <td><ul><li>No se pueden cumplir todas las políticas de seguridad y cumplimiento</li><li>Sin propiedad sobre la infraestructura física</li><li>No se pueden hacer escenarios específicos raros</li></ul></td>
  </tr>
</table>

### **Nube privada**
✖  Cloud Provider  ✅ Own Datacenter  
**Caracteristicas claves**
- Todo se ejecuta en su propio centro de datos
- Se debe proporcionar autoservicio
- Tú mantienes el hardware

<table>
  <tr>
    <th>Ventajas</th>
    <th>Desventajas</th>
  </tr>
  <tr>
    <td><ul><li>Puede soportar cualquier escenario</li><li>Control total sobre la seguridad y la infraestructura</li><li>Puede cumplir con cualquier política de seguridad y cumplimiento</li></ul></td>
    <td><ul><li>Se requiere inversión inicial</li><li>Agilidad limitada restringida por la capacidad del servidor y las habilidades del equipo</li><li>Muy dependiente de las habilidades y la experiencia en TI</li></ul></td>
  </tr>
</table>

### **Nube híbrida**
✅ Cloud Provider  ✅ Own Datacenter  
**Caracteristicas claves**  
- Combina la nube pública y privada

<table>
  <tr>
    <th>Ventajas</th>
    <th>Desventajas</th>
  </tr>
  <tr>
    <td><ul><li>Gran flexibilidad</li><li>Puede ejecutar cualquier aplicación heredada en la nube privada</li><li>Puede utilizar la infraestructura existente</li><li>Cumplir con los requisitos de seguridad y cumplimientos</li><li>Puede aprovechar todos los beneficios de la nube pública</li></ul></td>
    <td><ul><li>Puede ser más caro</li><li>Complicado de manejar debido a un paisaje más grande</li><li>Más dependiente de las habilidades y la experiencia en TI de los tres modelos</li></ul></td>
  </tr>
</table>

## **Geografía, Regiones y Zonas de disponibilidad**
  * Products available by region: https://azure.microsoft.com/en-us/global-infrastructure/services/
  * 🌐 Azure Speed Test 2.0: http://azurespeedtest.azurewebsites.net/

### **Data Center**
- **Instalación física**.
- **Hosting** para grupo de **servidores** en red.
- Infraestructura propia de **energía**, **refrigeración** y **redes**.

<img src="Images/Data-center.png" alt="Data Center" width="300"/> 

### **Región**
- **Área geográfica** en el planeta.
- **Uno, pero generalmente más centros de datos** conectados con una **red de baja latencia** (<2 milisegundos).
- **Ubicación** para sus servicios.
- Algunos servicios están **disponibles solo en ciertas regiones**.
- Algunos servicios son **servicios globales**, por lo que no se asignan/implementan en una región específica.
- Disponible globalmente con más de **50+ regiones**.
- **Regiones gubernamentales** especiales (US DoD Central, US Gov Virginia, etc.).
- **Regiones asociadas** especiales (Este de China, Norte de China).

<img src="Images/Regions.png" alt="Regions" width="300"/> 

### **Zona de disponibilidad**
- **Característica regional**.
- Agrupación de instalaciones **separadas físicamente**.
- Diseñado para **proteger de fallas en el centro de datos**.
- Si la zona se cae, **otros continúan trabajando**.
- Dos **categorías** de servicio:
  - Servicios **zonales** (Máquinas Virtuales, Discos, etc.).
  - Servicios con **redundancia de zona** (SQL, Storage, etc.).
- **No todas** las regiones son **compatibles**.
- La **región** admitida **tiene tres o más zonas**.
- Una **zona** es **uno o más centros de datos**.

<img src="Images/Availability-zone.png" alt="Availability Zone" width="300"/> 

### **Pares de regiones**
- Cada **región** está **emparejada** con otra región, lo que la convierte en un par de regiones.
- Los **pares de regiones son estáticos** y no se pueden elegir.
- Cada par reside dentro de la **misma geografía**.`La excepción es Brazil South`.
- **Aislamiento físico** con al menos 300 millas de distancia (cuando sea posible).
- Algunos servicios tienen **replicación proporcionada por la plataforma**.
- **Actualizaciones planificadas** en los pares.
- **Residencia de datos** mantenida para recuperación ante desastres.
Algunos ejemplos de regiones pares: 

Región Par A|Región Par B
---|---
East US|West US
UK West|UK South
North Europe|West Europe

<img src="Images/Regions-pairs.png" alt="Region Pairs" width="300"/> 

### **Geografías**
- **Mercado discreto**
- Normalmente **contiene dos o más regiones**.
- Garantiza que se cumplan los requisitos de **residencia**, **soberanía**, **resiliencia** y **cumplimiento** de los **datos**.
- **Tolerante a fallas** para proteger de fallas en toda la región.
- Dividido en áreas : **Américas**, **Europa**, **Asia Pacífico**, **Oriente Medio** y **África**.
- Cada **región pertenece solo a una Geografía**.

## **Recursos, grupos de recursos y administrador de recursos**
### **Recurso Azure**
- Objeto **utilizado para administrar servicios** en Azure.
- Representa el **ciclo de vida del servicio**.
- Guardado como **definición JSON**.

<img src="Images/Resources.png" width="300"/>

### **Grupo de recursos**
- **Agrupación** de recursos.
- Contiene recursos **lógicamente relacionados**.
- Normalmente se organiza por
  - **Tipo**
  - **Ciclo de vida** (aplicación, entorno)
  - **Departamento**
  - **Facturación**,
  - **Ubicación** o
  - **combinación de esos**

<img src="Images/Resource-group.png" width="300"/>

### **Administrador de recursos**
- **Capa de gestión** para todos los recursos y grupos de recursos
- Lenguaje **unificado**.
- **Controla el acceso** y **los recursos**.

<img src="Images/Resource-manager.png" width="300"/>

### **Información adicional**
- Cada **recurso** debe estar en **uno y solo un grupo de recursos**.
- Los **grupos de recursos tienen su propia ubicación** asignada.
- Los recursos de los grupos de recursos pueden **residir en ubicaciones diferentes**.
- Los recursos **se pueden mover** entre los grupos de recursos.
- Los **grupos de recursos no se pueden anidar**.
- Organícese en función de las necesidades de su organización, pero tenga en cuenta
  - Facturación
  - Seguridad y gestión de acceso
  - Ciclo de vida de la aplicación

## **Servicios de cómputo**
### **Virtualización**
- Emulación de máquinas físicas
- Configuración de hardware virtual diferente por máquina/aplicación
- Diferentes sistemas operativos por máquina/aplicación
- Separación total de ambientes
  - sistemas de archivos,
  - servicios,
  - puertos,
  - middleware,
  - configuración

<img src="Images/Virtualization.png" width="300"/>

### **Maquinas virtuales**
- Infraestructura como servicio (IaaS)
- Control total sobre el sistema operativo y el software
- Soporta mercado e imágenes personalizadas
- El más adecuado para
  - Software personalizado que requiere una configuración de sistema personalizada
  - Escenarios de elevación y cambio
- Puede ejecutar cualquier aplicación/escenario
  - aplicaciones web y servicios web,
  - bases de datos,
  - aplicaciones de escritorio,
  - jumpboxes,
  - gateways, etc

<img src="Images/Azure-virtual-machines.png" width="300"/>

### **Conjuntos de escalado de máquinas virtuales**
- Infraestructura como servicio (IaaS)
- Conjunto de máquinas virtuales idénticas
- Funciones de escalado automático integradas
- Diseñado para cargas de trabajo manuales y de escalado automático, como servicios web,* procesamiento por lotes, etc.

<img src="Images/Azure-virtual-machine-scale-sets.png" width="300"/>

### **Contenedores**
- Usar el sistema operativo del host
- Emular el sistema operativo (las máquinas virtuales emulan el hardware)
- Ligero (sin O/S)
  - Esfuerzo de desarrollo
  - Mantenimiento
  - Requisitos de computación y almacenamiento
- Responda más rápido a los cambios de demanda
- Diseñado para casi cualquier escenario

<img src="Images/Containers.png" width="300"/>

### **Instancias de contenedores de Azure**
- La forma más sencilla y rápida de ejecutar un contenedor en Azure
- Plataforma como servicio
- Contenedores sin servidor
- Diseñado para
  - Servicios/aplicaciones web pequeñas y sencillas
  - Trabajos en segundo plano
  - Guiones programados

<img src="Images/Azure-container-instances.png" width="300"/>

### **Servicio Azure Kubernetes (AKS)**
- Plataforma de orquestación de contenedores de código abierto
- Plataforma como servicio
- Altamente escalable y personalizable
- Diseñado para implementaciones de contenedores a gran escala (¡cualquier cosa realmente!)

<img src="Images/Azure-kubernetes-service.png" width="300"/>

### **Servicio de aplicaciones(App Service)**
- Diseñado como servicio de aplicación web de nivel empresarial
- Plataforma como servicio
- Admite múltiples lenguajes de programación y contenedores

<img src="Images/App-service.png" width="300"/>

### **Funciones de Azure (aplicaciones de funciones)**
- Plataforma como servicio
- Serverless
- Dos modelos de alojamiento/precio
  - Consumo-plan basado
  - plan dedicado
- Diseñado para micro/nanoservicios

<img src="Images/Functions-apps.png" width="300"/>

### **Resumen**
- Máquinas virtuales (IaaS) - software personalizado, requisitos personalizados, muy especializado, alto grado de control
- Conjuntos de escalado de máquinas virtuales (IaaS) - cargas de trabajo de escalado automático para máquinas virtuales
- Instancias de contenedor (PaaS) - alojamiento de contenedor simple, fácil de comenzar
- Servicio Kubernetes (PaaS) - Plataforma de alojamiento de contenedores * altamente escalable y personalizable
- Servicios de aplicaciones (PaaS) - aplicaciones web, muchas funciones de alojamiento web empresarial *, fácil de comenzar
- Funciones (PaaS) (Función como servicio) (Serverless) - micro/nanoservicios, excelente precio basado en el consumo, fácil de comenzar

<img src="Images/Summary.png" width="300"/>

## **Servicios de red**
### **Redes Azure (Azure Networking)**
- Conecte la nube y las instalaciones
- Funcionalidad de red local

### **Red virtual de Azure (Azure Virtual Network)**
- Componentes de red aislados lógicamente
- Segmentado en una o más subredes
- Las subredes son secciones discretas
- Habilite la comunicación de los recursos entre sí, Internet y en las instalaciones
- Alcanzado a una sola región
- El emparejamiento de VNet permite la comunicación entre regiones
- Aislamiento, Segmentación, Comunicación, Filtrado, Enrutamiento

<img src="Images/Virtual-network.png" width="300"/>

### **Equilibrador de carga de Azure (Azure Load Balancer)**
- Incluso la distribución del tráfico
- Admite escenarios tanto entrantes como salientes
- Escenarios de alta disponibilidad
- Aplicaciones TCP (protocolo de control de transmisión) y UDP (protocolo de datagramas de usuario)
- Tráfico Interno y Externo
- Reenvío de puertos
- Alta escala con hasta millones de flujos
<div>
<img src="Images/Load-balancer.png" width="300"/>
<img src="Images/Load-balancer-2.png" width="300"/>
</div>

### **Puerta de enlace VPN**
- Tipo específico de puerta de enlace de red virtual para el tráfico local a Azure a través de la Internet pública

<img src="Images/VPN-gateway.png" width="300"/>

### **Puerta de enlace de aplicaciones**
- Equilibrador de carga de tráfico web
- cortafuegos de aplicaciones web
- Redirección
- Afinidad de sesión
- Enrutamiento de URL
- Terminación SSL

<div>
<img src="Images/Application-gateway.png" width="300"/>
<img src="Images/Application-gateway-2.png" width="300"/>
<img src="Images/Application-gateway-3.png" width="300"/>
</div>

### **Red de entrega de contenidos**
- Definir contenido
- Minimizar la latencia
- POP (puntos de presencia) con muchas ubicaciones

<div>
<img src="Images/Content-delivery-network.png" width="300"/>
<img src="Images/Content-delivery-network-2.png" width="300"/>
</div>

## **Servicios de almacenamiento**
### **Tipos de datos**
- **Estructurado**: datos que se pueden representar mediante tablas con un esquema muy estricto. Cada fila debe seguir un esquema definido. Algunas tablas tienen relaciones definidas entre ellas. Normalmente se utiliza en bases de datos relacionales.  
- **Semiestructurado**: datos que se pueden representar mediante tablas pero sin un esquema estricto definido.  
Las filas solo deben tener un identificador de clave único.  
- **Sin estructura**: cualquier archivo en cualquier formato. Como archivos binarios, archivos de aplicaciones, imágenes, películas, etc.  

<img src="Images/Types-of-data.png" width="300"/>

### **Cuenta de almacenamiento**
- Grupo de servicios que incluyen
  - almacenamiento de blobs,
  - almacenamiento en cola,
  - almacenamiento de tablas y
  - almacenamiento de archivos
- Se utiliza para almacenar
  - archivos,
  - mensajes, y
  - datos semiestructurados
- Altamente escalable (hasta petabytes de datos)
- Muy duradero (99,999999999 % - 11 nueves, hasta 16 nueves)
- Más barato por GB de almacenamiento

<img src="Images/Storage-account.png" width="150"/>

### **Almacenamiento de blobs (Blob Storage)**
- BLOB – objeto grande binario – archivo
- Diseñado para el almacenamiento de archivos de cualquier tipo
- Tres niveles de almacenamiento
  - Hot: datos de acceso frecuente
  - Cool: datos a los que se accede con poca frecuencia (menor disponibilidad, alta durabilidad)
  - Archive: rara vez (si es que alguna vez) se accede a los datos

<img src="Images/Blob-storage.png" width="300"/>

### **Almacenamiento en cola (Queue Storage)**
- Almacenamiento de pequeños datos (mensajes)
- Diseñado para procesamiento asíncrono escalable

<div>
<img src="Images/Queue-storage.png" width="150"/>
<img src="Images/Queue-storage-2.png" width="150"/>
<img src="Images/Queue-storage-3.png" width="150"/>
</div>

### **Almacenamiento de tablas (Table Storage)**
- Almacenamiento para datos semiestructurados (NoSQL)
  - Sin necesidad de uniones foráneas, claves foráneas, relaciones o esquemas estrictos
  - Diseñado para un acceso rápido
- Muchas interfaces de programación y SDK

<img src="Images/Table-storage.png" width="300"/>

### **Almacenamiento de archivos (File Storage)**
- Almacenamiento para archivos a los que se accede a través de protocolos de unidades compartidas
- Diseñado para ampliar los recursos compartidos de archivos en las instalaciones o implementar escenarios de elevación y cambio

<img src="Images/File-storage.png" width="300"/>

### **Almacenamiento de disco (Disk Storage)**
- Emulación de disco en la nube
- Almacenamiento persistente para máquinas virtuales
- Diferente
  - tamaños,
  - tipos (SSD, HDD)
  - niveles de rendimiento
- El disco puede ser administrado o no administrado

<img src="Images/Disk-storage.png" width="100"/>

## **Servicios de bases de datos**
### **Tipos de datos en las BD**
Se explicó anteriormente. Revisar [Tipos de datos](#tipos-de-datos)
### **Cosmos DB**
- Servicio de base de datos NoSQL (datos semiestructurados) distribuido globalmente
- Sin esquema
- Múltiples API (SQL, MongoDB, Cassandra, Gremlin, Table Storage)
- Diseñado para
  - Aplicaciones de alta capacidad de respuesta (en tiempo real) con respuestas de latencia muy baja <10 ms
  - Aplicaciones multirregionales

<div>
<img src="Images/Cosmos-db.png" width="300"/>
<img src="Images/Cosmos-db-2.png" width="300"/>
</div>

### **SQL Database**
- Servicio de **base de datos relacional** en la nube (PaaS) (DBaaS - Database as a Service)
- **Servicio de datos estructurados** definido mediante esquema y relaciones
- **Capacidades de consulta enriquecidas** (SQL)
- Base de datos de **alto rendimiento**, fiable, totalmente gestionada y segura para la creación de aplicaciones

<div>
<img src="Images/SQL-database.png" width="300"/>
<img src="Images/SQL-server.png" width="300"/>
</div>

### **Azure SQL product family**
- Azure **SQL Database**: base de datos relacional confiable basada en SQL Server
- Azure **Database for MySQL**: versión de Azure SQL para el motor de base de datos MySQL
- Azure **Database for PostgreSQL**: versión de Azure SQL para el motor de base de datos de PostgreSQL
- **Instancia administrada de Azure SQL**: SQL Server completo administrado por un proveedor de la nube
- Azure **SQL en VM**: SQL Server completo en IaaS
- Azure **SQL DW (Synapse)**: versión de procesamiento paralelo masivo (MPP) de SQL Server

<img src="Images/Azure-sql.png" width="300"/>

## **Azure Marketplace**
- Piense en ello como una "Tienda Azure" donde compra servicios y soluciones para la plataforma Azure
- Cada producto es una plantilla que contiene uno o varios servicios
- Los productos son entregados por proveedores propios y externos.
- Las soluciones pueden aprovechar todas las categorías de servicios como IaaS, PaaS y SaaS

<img src="Images/Marketplace.png" width="300"/>

## **Servicios IoT**
Internet de las cosas (**IoT**) es una red de dispositivos conectados a Internet (**dispositivos IoT**) integrados en objetos cotidianos que permiten enviar y recibir datos, como **configuraciones** y **telemetría**.  
<img src="Images/Iot.png" width="300"/>

### **Azure IoT Hub**
- Servicio gestionado para comunicación bidireccional
- Plataforma como servicio (PaaS)
- Altamente seguro, escalable y confiable
- Se integra con una gran cantidad de servicios de Azure
- SDK programables para lenguajes populares (C, C#, Java, Python, Node.js)
- Múltiples protocolos (HTTPS, AMQP, MQTT)  

<img src="Images/Iot-hub.png" width="300"/>

### **Azure IoT Central**
- Plataforma de aplicaciones IoT: software como servicio (SaaS)
- Plantillas de aplicaciones específicas de la industria
- No se requieren conocimientos técnicos profundos
- Servicio de conexión, gestión y monitorización de dispositivos IoT
- Altamente seguro, escalable y confiable
- Construido sobre el servicio IoT Hub y más de 30 servicios más  

<img src="Images/Iot-central.png" width="300"/>

### **Azure Sphere**
- Soluciones seguras de IoT de extremo a extremo
  - Chips certificados por Azure Sphere (unidades de microcontrolador - MCU)
  - Sistema operativo Azure Sphere basado en Linux
  - Comunicación de dispositivo a nube de confianza de Azure Security Service 
 
<img src="Images/Sphere.png" width="300"/>

## **Servicios Big Data & Analytics**
Big Data es un campo de la tecnología que ayuda con la extracción, el procesamiento y el análisis de información que es demasiado grande o compleja para ser tratada por el software tradicional.  
**La regla de las tres V**
Los grandes datos suelen tener una de las siguientes características  
- **Velocidad**: qué tan rápido ingresan los datos o qué tan rápido los estamos procesando
  - Batch
  - Periódico
  - Casi en tiempo real
  - Tiempo real
- **Volumen**: cuántos datos estamos procesando
  - Megabytes
  - Gigabyte
  - Terabytes
  - Petabytes
- **Variedad**: cuán estructurados/complejos son los datos
  - Tables
  - bases de datos
  - Foto, Audio
  - Vídeo, Redes Sociales

### **Azure Synapse Analytics**
- Plataforma de análisis de big data (PaaS)
- Múltiples componentes
  - Spark
  - Synapse SQL
    - Grupos de SQL (dedicados: pago por rendimiento aprovisionado)
    - SQL bajo demanda (ad-hoc: pago por TB procesados)
  - Synapse Pipelines (Data Factory - ETL)
  - Studio (experiencia unificada)

<img src="Images/Synapse-analytics.png" width="300"/>

### **Azure HDInsight**
- Plataforma flexible multipropósito de big data (PaaS)
- Múltiples tecnologías compatibles (Hadoop, Spark, Kafka, HBase, Hive, Storm, Machine Learning)

<img src="Images/HDInsight.png" width="300"/>

### **Azure Databricks**
- Plataforma de colaboración de big data (PaaS)
- Espacio de trabajo unificado para portátiles, clústeres, datos, administración de acceso y colaboración
- Basado en Apache Spark
- Se integra muy bien con los servicios de datos comunes de Azure

<img src="Images/Databricks.png" width="300"/>

## **Servicios de IA**
**¿Qué es la Inteligencia Artificial?**  
La inteligencia artificial (IA) es la simulación de la inteligencia y las capacidades humanas mediante un software informático.  
**¿Qué es el aprendizaje automático?**  
El aprendizaje automático es una subcategoría de la IA en la que se "enseña" un software de computadora a sacar conclusiones y hacer predicciones a partir de los datos.  
### **Azure Machine Learning**
- Plataforma basada en la nube para crear, administrar y publicar modelos de aprendizaje automático
- Plataforma como servicio (PaaS)
- Espacio de trabajo de aprendizaje automático: recurso de nivel superior
- Machine Learning Studio: portal web para desarrollo extremo a extremo
- Características
  - Cuadernos: usando Python y R
  - ML automatizado: ejecute múltiples combinaciones de algoritmos/parámetros, elija el mejor modelo
  - Diseñador: interfaz gráfica para el desarrollo sin código
  - Datos y computación: administración de recursos de almacenamiento y computación
  - Pipelines: orqueste tareas de capacitación, implementación y administración de modelos

<img src="Images/Machine-learning.png" width="300"/>

## **Servicios serverless computing**
La computación sin servidor es un entorno de ejecución alojado en la nube que permite a los clientes ejecutar sus aplicaciones en la nube mientras abstraen por completo la infraestructura subyacente.
### **Azure Functions**
- Plataforma de codificación sin servidor (Funciones como servicio, FaaS)
- Diseñado para arquitecturas de nanoservicios y aplicaciones basadas en eventos
- Escala hacia arriba y hacia abajo muy rápidamente
- Altamente escalable
- Admite lenguajes y marcos populares (.NET y .NET Core, Java, Node.js, Python, PowerShell, etc.)

<img src="Images/Azure-functions-apps.png" width="300"/>

### **Azure Logic Apps**
- Servicio de integración empresarial sin servidor (PaaS)
- Más de 200 conectores para servicios populares
- Diseñado para la orquestación de
  - Procesos de negocios,
  - flujos de trabajo de integración para aplicaciones, datos, sistemas y servicios
- Solución sin código

<img src="Images/Azure-logics-apps.png" width="300"/>

### **Azure Event Grid**
- Servicio de enrutamiento de eventos sin servidor completamente administrado
- Utiliza el modelo de publicación-suscripción
- Diseñado para aplicaciones basadas en eventos y casi en tiempo real
- Admite docenas de eventos integrados de los servicios de Azure más comunes

<img src="Images/Azure-event-grid.png" width="300"/>

## **Soluciones DevOps**
**DevOps** es un conjunto de prácticas que combinan tanto el desarrollo (Dev) como las operaciones (Ops).  
DevOps tiene como objetivo **acortar el ciclo de vida del desarrollo** al proporcionar capacidades de **integración y entrega continuas** (CI/CD) al tiempo que garantiza una **alta calidad** de los entregables.

### **Azure DevOps**
- Colección de servicios para construir soluciones usando prácticas DevOps
- Servicios incluidos
  - Tableros: trabajo de seguimiento
  - Canalizaciones: creación de flujos de trabajo de CI/CD (creación, prueba e implementación de aplicaciones)
  - Repos: colaboración de código y control de versiones con Git
  - Planes de prueba: pruebas manuales y exploratorias
  - Artefactos: gestione los entregables del proyecto
- Ampliable con Marketplace: más de 1000 aplicaciones disponibles
- Evolucionado de TFS (Team Foundation Server), a través de VSTS (Visual Studio Team Services)

<img src="Images/Azure-devops.png" width="300"/>

### **Azure DevTest Labs**
- Servicio de creación de entornos sandbox para desarrolladores/testers (PaaS)
- Configuración rápida de máquinas virtuales autogestionadas
- Plantillas preconfiguradas para máquinas virtuales
- Muchos artefactos adicionales (herramientas, aplicaciones, acciones personalizadas)
- Políticas de laboratorio (cuotas, tamaños, apagado automático)
- Comparta y automatice laboratorios a través de imágenes personalizadas
- Complementos/API/herramientas prefabricados para la automatización de canalización de CI/CD

<img src="Images/Azure-devtest-labs.png" width="300"/>
