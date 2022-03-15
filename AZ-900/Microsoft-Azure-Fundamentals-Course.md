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
    - [Data Center](#data-center)
    - [**Región**](#región)
    - [**Zona de disponibilidad**](#zona-de-disponibilidad)
    - [**Pares de regiones**](#pares-de-regiones)
    - [**Geografías**](#geografías)
  - [**Recursos, grupos de recursos y administrador de recursos**](#recursos-grupos-de-recursos-y-administrador-de-recursos)
    - [**Recurso Azure**](#recurso-azure)
    - [**Grupo de recursos**](#grupo-de-recursos)
    - [**Administrador de recursos**](#administrador-de-recursos)
    - [**Información adicional**](#información-adicional)
  - [**Servicios de cómputo | VMs, VM Scale Set, App Service, Functions, ACI, AKS**](#servicios-de-cómputo--vms-vm-scale-set-app-service-functions-aci-aks)
    - [**Virtualización**](#virtualización)
    - [**Maquinas virtuales**](#maquinas-virtuales)
    - [**Conjuntos de escalado de máquinas virtuales**](#conjuntos-de-escalado-de-máquinas-virtuales)
    - [**Contenedores**](#contenedores)
    - [**Instancias de contenedores de Azure**](#instancias-de-contenedores-de-azure)
    - [**Servicio Azure Kubernetes (AKS)**](#servicio-azure-kubernetes-aks)
    - [**Servicio de aplicaciones(App Service)**](#servicio-de-aplicacionesapp-service)
    - [**Funciones de Azure (aplicaciones de funciones)**](#funciones-de-azure-aplicaciones-de-funciones)
    - [**Resumen**](#resumen)
  - [**Servicios de red | Virtual Network, VPN Gateway, CDN, Load Balancer, App GW**](#servicios-de-red--virtual-network-vpn-gateway-cdn-load-balancer-app-gw)
    - [**Redes Azure (Azure Networking)**](#redes-azure-azure-networking)
    - [**Red virtual de Azure (Azure Virtual Network)**](#red-virtual-de-azure-azure-virtual-network)
    - [**Equilibrador de carga de Azure (Azure Load Balancer)**](#equilibrador-de-carga-de-azure-azure-load-balancer)
    - [**Puerta de enlace VPN**](#puerta-de-enlace-vpn)
    - [**Puerta de enlace de aplicaciones**](#puerta-de-enlace-de-aplicaciones)
    - [**Red de entrega de contenidos**](#red-de-entrega-de-contenidos)

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

Ventajas|Desventajas
---|---
<ul><li>Sin CapEx</li><li>Alta disponibilidad</li><li>Agilidad</li><li>Precios por pago de uso</li><li>Sin mantenimiento de hardware</li><li>No se requieren habilidades técnicas profundas</li></ul>|<ul><li>No se pueden cumplir todas las políticas de seguridad y cumplimiento</li><li>Sin propiedad sobre la infraestructura física</li><li>No se pueden hacer escenarios específicos raros</li></ul>

### **Nube privada**
✖  Cloud Provider  ✅ Own Datacenter  
**Caracteristicas claves**
- Todo se ejecuta en su propio centro de datos
- Se debe proporcionar autoservicio
- Tú mantienes el hardware

Ventajas|Desventajas
---|---
<ul><li>Puede soportar cualquier escenario</li><li>Control total sobre la seguridad y la infraestructura</li><li>Puede cumplir con cualquier política de seguridad y cumplimiento</li></ul> | <ul><li>Se requiere inversión inicial</li><li>Agilidad limitada restringida por la capacidad del servidor y las habilidades del equipo</li><li>Muy dependiente de las habilidades y la experiencia en TI</li></ul>

### **Nube híbrida**
✅ Cloud Provider  ✅ Own Datacenter  
**Caracteristicas claves**  
- Combina la nube pública y privada

Ventajas|Desventajas
---|---
<ul><li>Gran flexibilidad</li><li>Puede ejecutar cualquier aplicación heredada en la nube privada</li><li>Puede utilizar la infraestructura existente</li><li>Cumplir con los requisitos de seguridad y cumplimientos</li><li>Puede aprovechar todos los beneficios de la nube pública</li></ul> | <ul><li>Puede ser más caro</li><li>Complicado de manejar debido a un paisaje más grande</li><li>Más dependiente de las habilidades y la experiencia en TI de los tres modelos</li></ul>

## **Geografía, Regiones y Zonas de disponibilidad**
  * Products available by region: https://azure.microsoft.com/en-us/global-infrastructure/services/
  * 🌐 Azure Speed Test 2.0: http://azurespeedtest.azurewebsites.net/

### Data Center
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

## **Servicios de cómputo | VMs, VM Scale Set, App Service, Functions, ACI, AKS**
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

## **Servicios de red | Virtual Network, VPN Gateway, CDN, Load Balancer, App GW**
### **Redes Azure (Azure Networking)**
- Conecte la nube y las instalaciones
- Funcionalidad de red local

<img src="Images/" width="300"/>


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
<img src="Images/Load-Load-balancer-2.png" width="300"/>
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