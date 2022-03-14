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
<ul><li>Puede soportar cualquier escenario</li><li>Control total sobre la seguridad y la infraestructura
</li><li>Puede cumplir con cualquier política de seguridad y cumplimiento</li></ul>|<ul><li>Se requiere inversión inicial</li><li>Agilidad limitada restringida por la capacidad del servidor y las habilidades del equipo</li><li>Muy dependiente de las habilidades y la experiencia en TI</li></ul>

### **Nube híbrida**
✅ Cloud Provider  ✅ Own Datacenter 
**Caracteristicas claves** 
- Combina la nube pública y privada

Ventajas|Desventajas
---|---
<ul><li>Gran flexibilidad</li><li>Puede ejecutar cualquier aplicación heredada en la nube privada</li><li>Puede utilizar la infraestructura existente
</li><li>Cumplir con los requisitos de seguridad y cumplimiento
</li><li>Puede aprovechar todos los beneficios de la nube pública
Desventajas</li></ul>|<ul><li>Puede ser más caro
</li><li>Complicado de manejar debido a un paisaje más grande
</li><li>Más dependiente de las habilidades y la experiencia en TI de los tres modelos</li></ul>
