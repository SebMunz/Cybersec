
# TIPOS DE CONEXIONES
_Conexiones comunes que se encuentran en el area y sus impactos_

> __Cable__

Ethernet siendo la conexión mas común.
Transmite datos de manera segura y rápida entre dispositivos usando cables Cat5 o superior.
Se le considera más confiable y segura que el inalámbrico gracias a la menor vulnerabilidad a interferencias y accesos no autorizados.

---

> __USB__

Utilizado ampliamente para conectar periféricos a computadores. Si bien es conveniente, plantea riesgos de seguridad al conectar dispositivos no confiables.
Es de suma importancia garantizar que son dispositivos de confianza.

---

> __Inalámbricas__

Siendo el Wi-Fi el más común, ofrece flexibilidad y movilidad sin cable físico. Introduce riesgos de seguridad comunes. Para mitigar algunos riesgos, se recomienda el cifrado WPA3, el uso de contraseñas seguras y actualizaciones del firmware del router.
Wi-Fi es conveniente en su uso por su conexión fácil de configurar y su escalabilidad.

###### Algunos riesgos comunes:
- Escuchas: Interceptación de datos transmitidos
- Puntos de Acceso Falsos
- Man in the middle: Interceptación de datos entre un dispositivo en la red, alterando los datos

###### Mejores prácticas para mitigar riesgos:
- Cifrado fuerte
- Cambiar credenciales predeterminadas
- Actualizar firmware del router
- Red de invitados
- Desactivar WPS
- Usar VPN

---

> __Bluetooth__

Conexión de corto alcance entre dispositivos. Conveniente pero no excento de ataques como Bluesnarfing, BlueBorne y Bluejacking. Para mitigar riesgos se recomienda mantener dispositivos actualizados, utilziar bluetooth 4.0 (mínimo) y desactivarlo cuando en desuso.
Opera en la frecuencia 2.4 GHz.

###### Ataques bluetooth
- Bluejacking: Comunicación no solicitada
  - Mitigación: Desactivar visibilidad y rechazar conexiones no solicitadas
- Bluesnarfing: Acceso al dispositivo de forma maliciosa a través de una vulnerabilidad en el protocolo
  - Mitigación: Mantener actualizado, desactivar visibilidad si no está en uso
- BlueBorne: Vulnerabilidad crítica que explota debilidades del protocolo. Se usa para ganar control del dispositivo infectado e infectar otros dispositivos cercanos.
  - Mitigación: Mantener actualizado, desactivar Bluetooth si no está en uso



---

> __Enmascaramientos__

O conexiones de red. Los VPN son túneles seguros que crean conexiones de red privada sobre una red pública. De esta forma se protege la información de interceptaciones. Útiles al usar Wi-Fi público. Utilizar proovedores confiables.

---

> __P2P__

Peer-to-Peer. Conexión descentralizada, común en servicios de intercambio de archivos. Sin medidas de seguridad adecuadas presentan un inmenso riesgo. Evitar los servicios no confiables y nunca compartir información sensible en ellos.

---

> __NFC__

_No confundir EMV, o el chip de las tarjetas, similar uso y similar tecnología, diferentes actores detras de ellas_

Near Field Communication (Comunicación de campo cercano), deriva del área de las RFID (radio-frequency identification). Tecnología inalámbrica de corto alcance (PAN - Personal Area Network). Opera a 13.56 MHz, muy utilizado en aplicaciones como pagos sin contacto y control de acceso.
Se conectan a través de etiquetas y lectores.
Tiene tres modos: Lector/Escritor, P2P y Emulación de tarjeta
- ###### Lector/Escritor
  - Permite al dispositivo leer o escribir en etiquetas NFC, como posters.
- ###### P2P
  - Permite que dos dispositivos intercambien información, como compartir datos de contacto
- ###### Emulación de Tarjeta
  - Permite que un dispositivo actué como tarjeta inteligente, como facilitar pagos

Si bien es muy seguro, a pesar de su conveniencia presenta diversos riesgos de seguridad como la manipulación de datos por terceros y accesos no autorizados.
Para mitigar estos riesgos se recomienda:
- Mantener firmware y aplicaciones actualizadas
- Uso de contraseñas fuertes
- Desactivar si no está en uso
- Escanear etiquetas NFC de confianza
- Usar aplicaciones confiables y seguras para las transacciones

_NOTA: Ver FLIPPER ZERO como herramienta para PenTest_

---

> IR o __Infrarroja__

Utiliza ondas de luz para transmitir datos. Común en comunicación de corto alcance.
Usado en controles remotos, teclados y mouse inalámbricos y comunicación entre computadores e impresoras.
Es privado (no atraviesa paredes), de fácil configuración y de bajo consumo.
Sin embargo, su rango es limitado, tiene baja transferencia de datos y su transmisión es en línea de visión (directa).
A pesar de todo esto, igual se debe tener consideraciones de seguridad:
- Cifrado
- Autenticación
- Seguridad física
  
Algunos ataques a considerar:
- Replay Attack: transmisión previamente grabada y legítima que se reproduce posteriormente para engañar
- Spoofing: emular un dispositivo autorizado para ganar acceso
- Interceptación: A través de dispositivos especializados se puede interceptar y reproducir la señal
- Ingeniería Social: persuadir a la víctima para realizar acciones no seguras, como aceptar conexiones desconocidas
