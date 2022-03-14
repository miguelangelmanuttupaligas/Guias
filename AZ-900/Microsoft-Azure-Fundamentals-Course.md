# Microsoft Azure Fundamentals Course
## Temario
- [Microsoft Azure Fundamentals Course](#microsoft-azure-fundamentals-course)
  - [Temario](#temario)
  - [Cloud Computing y Conceptos clave](#cloud-computing-y-conceptos-clave)
    - [Cloud Computing](#cloud-computing)
    - [Conceptos clave](#conceptos-clave)
  - [Principios de economía de escala](#principios-de-economía-de-escala)
  - [CapEx vs OpEx y sus diferencias](#capex-vs-opex-y-sus-diferencias)
  - [Modelo basado en el consumo](#modelo-basado-en-el-consumo)

## Cloud Computing y Conceptos clave
### Cloud Computing
Modelo de prestación de servicios a través de internet (nube). Esto incluye pero no se limita a
- **Compute power** es decir, servidores como Windows, Linux, entornos de alojamiento, etc.
- **Storage** como archivos y/o bases de datos
- **Networking** en azure pero también fuera cuando se conecta a la red de su empresa
- **Analytics** servicios de visualización y datos de telemetría  
<img src="Images/Cloud-Computing.png" alt="Cloud-Computing" width="300"/>

### Conceptos clave
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

## Principios de economía de escala
El principio de economías de escala establece que a medida que las empresas crecen, se vuelven más efectivas en la gestión de operaciones compartidas. Ya sea recursos humanos y contratación, impuestos, contabilidad, operaciones internas, marketing, grandes compras a través de contratos que significan mejores descuentos, etc.  
Por eso,las empresas pueden ahorrar/ganar más, lo que a cambio les permite reducir el costo de sus servicios para sus clientes. Esto se llama **'precio por unidad'**.  
No es posible ir a 0 porque, al final, se debe ejecutar alguna infraestructura subyacente para proporcionar los servicios. Pero cuanto mayor sea la escala, más beneficios se pueden transferir a los clientes.  
De hecho, en la escala actual, Microsoft ya puede ofrecer múltiples servicios de forma gratuita debido a lo pequeña que es una fracción del costo para ellos.  
<div>
    <img src="Images/Economies-of-scale.png" alt="Economies-of-scale" width="300"/>  
    <img src="Images/Economies-of-scale-2.png" alt="Economies-of-scale-2" width="300"/>  
</div> 

## CapEx vs OpEx y sus diferencias
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

## Modelo basado en el consumo
El modelo basado en el consumo es un modelo de precios que se utiliza en la nube para que a los clientes solo se les cobre en función de su uso de recursos.  
Este modelo se caracteriza por  

- **Sin costo inicial asociado**
- **No se desperdician recursos** como tal, *no se incurre en cargos por recursos no utilizados*. No utilizado en este caso es diferente por servicio. Por ejemplo, Se considera que se usa el almacenamiento de blobs que almacena cualquier dato, ya que consume el espacio de almacenamiento. Las máquinas virtuales que se ejecutan consumen CPU, memoria y otros recursos incluso si no hay tráfico. Por lo tanto, se consideran utilizados y generarán cargos.
- **Paga por lo que necesitas**
- **Deja de pagar cuando no lo haces**  
**El consumo** es la métrica virtual que se usa para calcular cuánto se usó cada recurso (servicio) en Azure. Cada servicio tiene muchas métricas más pequeñas que rastrean su consumo para ofrecer el mejor modelo de precios posible. Esas métricas se rastrean en un nivel muy granular.  
<img src="Images/Consumption-based-model.png" alt="CapEx" title="CapEx" width="300"/> 

[Consumption based Model - AZ-900 - Chapter Demo](https://youtu.be/NdqncsMtryY?list=PLGjZwEtPN7j-Q59JYso3L4_yoCjj2syrM) 
