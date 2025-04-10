### **Actividad: Computación en la nube**
***
Esta actividad se orienta a estudiantes de desarrollo de software que deseen entender los fundamentos de la computación en la nube.
##### A. Cuestionario
1. **Motivaciones para la nube**
    - (a) ¿Qué problemas o limitaciones existían antes del surgimiento de la computación en la nube y cómo los solucionó la centralización de servidores en data centers?
		- **Con el uso de la  computación en la nube se reducen los costos en la infraestructura:** ya no se tiene que invertir en hardware o incluso construir un gran data center, mucho menos contratar un equipo IT para administrarlo.
		- **Seguridad de los datos:** Los proveedores de servicios cloud ofrecen varias características para proteger datos como permisos granulares. También implementan protecciones para la data que procesan como autenticación, control de acceso y encriptación.
		- **Escalabilidad:** La computación en la nube permite a las empresas escalar de acorde a sus necesidades en cierto instante de tiempo. También se puede usar infraestructura más "pequeña" según la demanda lo cual reduce los costos. 
		- **Movilidad:** Los usuarios pueden trabajar desde cualquier lugar del mundo con un par de clicks siempre y cuando se tenga acceso a internet.
		
    - (b) ¿Por qué se habla de “The Power Wall” y cómo influyó la aparición de procesadores multi-core en la evolución hacia la nube?
	    - The Power Wall se refiere a la dificultad de aumentar el rendimiento de una CPU ya que esto conlleva a grandes consumos de energías y disipación de calor no costeable. 
		- Los procesadores multi-core permiten la elasticidad a los usuarios de los servicios nube, ya que se puede asignar un cierto número de núcleos de acuerdo a la demanda.
		- Estos nuevos procesadores también so beneficiosos para los proveedores de servicios nube pues hacen el consumo de energía y disipación del calor mas eficientes.
    
2. **Clusters y load balancing**
    - (a) Explica cómo la necesidad de atender grandes volúmenes de tráfico en sitios web condujo a la adopción de clústeres y balanceadores de carga.
	    Atender grandes volúmenes de tráfico condujo a la adopción de clústeres de servidores porque se necesitaba distribuir este tráfico. Los balanceadores de carga se encargan de la forma en que este se distribuyen. Los clústeres también brindan seguridad pues no se depende de un solo servidor para que la web este en pie.
    - (b) Describe un ejemplo práctico de cómo un desarrollador de software puede beneficiarse del uso de load balancers para una aplicación web.
	    Es 24 de diciembre y hay un gran tráfico en una tienda online. El load balancer distribuye el tráfico en distintos servidores reduciendo la latencia y mejorando la experiencia de usuario. Si algún nodo no está activo el tráfico se redirige a los que sí lo están dándole alta disponibilidad a la tienda.
3. **Elastic computing**
    - (a) Define con tus propias palabras el concepto de Elastic Computing.
	    Elastic Computing es la habilidad de un sistema para escalar sus recursos según la demanda.
    - (b) ¿Por qué la virtualización es una pieza clave para la elasticidad en la nube?
	    La virtualización abstrae los recursos como la memoria, la CPU o el almacenamiento lo cual facilita el escalado sin interrupciones asignando más recursos o creando mas VMs.
    - (c) Menciona un escenario donde, desde la perspectiva de desarrollo, sería muy difícil escalar la infraestructura sin un entorno elástico.
	    Una tienda online recibe un gran tráfico debido a la introducción de un producto novedoso, pero los servidores no están preparados para este. Se debería haber preparado con anticipación, pero esto es riesgoso porque si el producto no vendiese se habría invertido en infraestructura innecesariamente.

4. **Modelos de servicio (IaaS, PaaS, SaaS, DaaS)**
    - (a) Diferencia cada uno de estos modelos. ¿En qué casos un desarrollador optaría por PaaS en lugar de IaaS?
    - (b) Enumera tres ejemplos concretos de proveedores o herramientas que correspondan a cada tipo de servicio.
	    - **IaaS:** Proporciona recursos virtualizados como servidores, redes y almacenamiento. El proveedor mantiene la infraestructura física. Ejemplos: AWS EC2, Microsoft Azure VM y Linode.
	    - **PaaS:** Ofrece una plataforma para el desarrollo de una aplicación. El usuario no diseña ni mantiene la infraestructura. Ejemplos: Microsoft App Services, Google App Engine y Heroku.
	    - **SaaS:** Ofrece una aplicación completa en la nube. Ejemplos: Microsoft 365, Gmail y Dropbox.
	    - **DaaS:** Ofrece Escritorios completos en nube accesibles desde cualquier dispositivo. Ejemplos: VMware Horizon Cloud, Azure Virtual Desktop y Amazon WorkSpaces.
	    Un desarrollador optaría por Paas en lugar de IaaS cuando no quiera diseñar la infraestructura y enfocarse solamente en el desarrollo  de la aplicación.

5. **Tipos de nubes (Pública, Privada, Híbrida, Multi-Cloud)**
    - (a) ¿Cuáles son las ventajas de implementar una nube privada para una organización grande?
	    - Control  sobre la infraestructura y los recursos.
	    - Son más costo efectivos para empresas con cargas de trabajo poco variantes.
	    - Reduce los riesgos asociados a entornos compartidos.
	    - Facilita el cumplimiento de normas específicas.
    - (b) ¿Por qué una empresa podría verse afectada por el “provider lock-in”?
	    - Porque el proveedor ofrece servicios altamente especializados difíciles de encontrar en otras empresas.
	    - No poder cambiarse a otro proveedor debido a contratos a largo plazo.
	    - Costos elevados de cambio. Algunos proveedores podrían hacer difícil la migración a otro.
    - (c) ¿Qué rol juegan los “hyperscalers” en el ecosistema de la nube?
		- Perseguir los siguientes objetivos: Escalabilidad para los usuarios, transparencia del costo con el uso de "pay-per-user" e innovar en nuevas tecnologías nube.

#### B. Actividades de investigación y aplicación

1. **Estudio de casos**
    - Busca dos o tres casos de empresas (startups o grandes organizaciones) que hayan migrado parte de su infraestructura a la nube. Describe:
        1. Sus motivaciones para la migración.
        2. Los beneficios obtenidos (por ejemplo, reducción de costos, escalabilidad, flexibilidad).
        3. Los desafíos o dificultades enfrentadas (ej. seguridad, cumplimiento normativo).
        
| Empresa                     | Motivación                                                                             | Beneficios                                                                                                                       | Desafíos                                                                                                                                     |
| --------------------------- | -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------- |
| Spotify                     | Enfocarse en características innovadoras, grandes volúmenes de datos y alcance global. | Libero recursos para concentrarse en features como análisis de datos, recomendaciones personalizadas y descubrimiento de música. | Evaluar entre diferentes estrategias: multi-provider, hybrid y single-provider.                                                              |
| General Electric Healthcare | Transferir sus datos y plataformas de análisis.                                        | Beneficios significativo en costos al usar herramientas nube como el pago por uso.                                               | Migrar eficientemente los datos y cumplir con los deadlines del proyecto. También hubo un desafío al migrar una gran variedad de data types. |

        
        
2. **Comparativa de modelos de servicio**
    - Realiza un cuadro comparativo en el que muestres las **responsabilidades** del desarrollador, del proveedor y del equipo de operaciones en los distintos modelos (IaaS, PaaS, SaaS).
    - Incluye aspectos como: instalación de S.O., despliegue de aplicaciones, escalado automático, parches de seguridad, etc.

| Servicio | Proveedor                                                                                                                    | Ops team                                                                                                                         | Desarrollador                                             |
| -------- | ---------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------- |
| IaaS     | Hardware, red, almacenamiento, servidores y virtualización                                                                   | configura el SO, aplica parches de seguridad, gestiona escalado automático, supervisa el rendimiento, y configura el middleware. | Despliega y gestiona la aplicación, y gestiona los datos. |
| PaaS     | Hardware, red, almacenamiento, servidores y virtualización, parches de seguridad, configura el SO y configura el middleware. | Gestiona el escalado automático, supervisa el rendimiento                                                                        | Despliega y gestiona la aplicación, y gestiona los datos. |
| SaaS     | Todo                                                                                                                         | -                                                                                                                                | Usa la aplicación                                         |


