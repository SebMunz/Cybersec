## Indicadores de compromiso (IoC) e Indicadores de ataque (IoA)

<u>Evidencias observadas</u>.
**Compromiso** indica "posible incidente de seguridad". Trazan evidencia vinculada a un ataque, como nombres de archivos asociados.
**Ataque** indica la serie de eventos observados de un incidente en tiempo real. Como el comportamiento de un atacante.

<u>Básicamente</u>:
**IoC** ayuda a identificar quién y qué de un ataque después de que ocurrió.
**IoA** es el por qué y cómo de un ataque en curso o desconocido.

**NO SIEMPRE SON CONFIRMACIÓN DE UN INCIDENTE**

---

## Pirámide del dolor

David J. Bianco creó el concepto de pirámide del dolor. Su objetivo es mejorar la forma en que se usan los IoC en la detección.
Ésta establece una relación entre IoC y el nivel de dificultad que los agentes de amenaza deben enfrentar, cuando los indicadores de compromiso son bloqueados por los equipos de seguridad.
![[bamsulxz.bmp]]
- Valores Hash:
	- Si logras obtener el hash de un archivo malicioso conocido en tu red, es relativamente sencillo escanear todo el entorno para descubrir el nivel de infección.
- Direcciones IP:
	- Relativamente sencillo identificar conexiones IP no confiables si es que mantenemos un monitoreo constante.
- Nombres de dominio:
	- Dada la infinidad de [[TOP LEVEL DOMAINS (TLD)]] que se pueden lograr, cuando un atacante usa este método, combinado con [[DOMAIN GENERATION ALGORITHMS (DGA)]] + [[DNS Fast Flux]], logran rotar por nombres múltiples de forma regular, dificultando su identificación.
- Artefactos de red:
	- Existe variedad maneras de configurar y manejar una red interna. El factor que más influye aquí es el cómo interactua el usuario con ellas. Multiplícalo por 100 o miles de usuarios en una empresa y tienes que encontrar todas las instancias de un archivo malicioso. Esto lo hace potencialmente dificil.
	  En red, es la evidencia observable creada por los agentes de amenaza en una red como [[User-Agent strings]]
- Artefactos de host:
	- Lo mismo que en red, pero en el host. Como por ejemplo, nombres de archivos creados por malware
- Herramientas:
	- Herramientas usadas por un agente de amenaza. A un nivel empresarial es muy díficil identificarlas. Si no tienes un artifacto en el host, ¿realmente hubo un ataque?, quizás sí pero para identificarlo debes primero encontrar un punto de partida.
- Tácticas, técnicas y procedimientos:
	- Aquí ya hablamos de metodologías y modus operandi del agente. Todo lo que observamos durante el incidente (o antes) para intentar determinar *qué*. Lo más probable es que en este nivel tengas que pasar a un modelo más preciso e intensivo, como el [[MITRE ATT&CK]]

