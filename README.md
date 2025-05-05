# IS-3.a..e-ACF

# ÍNDICE
- [¿Qué te ha parecido los temas tratados?](#qué-te-ha-parecido-los-temas-tratados)
- [¿Qué te ha parecido más útil para tu futuro puesto de trabajo en un equipo de seguridad?](#qué-te-ha-parecido-más-útil-para-tu-futuro-puesto-de-trabajo-en-un-equipo-de-seguridad)
- [¿Conocías todos los puntos tratados en la unidad? ¿Cuáles no?](#conocías-todos-los-puntos-tratados-en-la-unidad-cuáles-no)
- [¿Alguno te ha llamado especialmente la atención? ¿Por qué?](#alguno-te-ha-llamado-especialmente-la-atención-por-qué)
- [¿Descartarías algún punto de la unidad? ¿Cuál y por qué?](#descartarías-algún-punto-de-la-unidad-cuál-y-por-qué)
- [¿Has echado en falta algún tema?](#has-echado-en-falta-algún-tema)
- [Resumen de la unidad](#resumen-de-la-unidad)
    - [Recopilación y almacenamiento de evidencias digitales](#recopilación-y-almacenamiento-de-evidencias-digitales)
    - [Procedimiento y cadena de custodia](#procedimiento-y-cadena-de-custodia)
    - [Herramientas y ejemplos prácticos](#herramientas-y-ejemplos-prácticos)
    - [Marcos de investigación: MITRE ATT&CK y RE&CT](#marcos-de-investigación-mitre-attck-y-rect)
    - [Conclusiones](#conclusiones)

---

## ¿Qué te ha parecido los temas tratados?
Me han parecido temas absolutamente imprescindibles para cualquier persona que vaya a dedicarse profesionalmente a la ciberseguridad. La unidad va mucho más allá de la teoría, centrando la atención en la gestión real de incidentes, la importancia de la evidencia digital y la aplicación de marcos reconocidos internacionalmente como MITRE ATT&CK y RE&CT. Todo el enfoque del temario está orientado a que el alumno adquiera mentalidad de investigador y “forense digital”, destacando la importancia de procedimientos rigurosos, la documentación precisa y la preservación de la cadena de custodia. La visión práctica, basada en ejemplos y referencias normativas (como la RFC 3227), ayuda a entender la realidad de los equipos de respuesta a incidentes en empresas.

---

## ¿Qué te ha parecido más útil para tu futuro puesto de trabajo en un equipo de seguridad?
Sin duda, lo más útil ha sido la parte relacionada con la recopilación y almacenamiento de evidencias, y la gestión de la cadena de custodia, porque son habilidades fundamentales en cualquier investigación de incidentes. Además, el uso de frameworks como ATT&CK y RE&CT me ha parecido clave para estructurar y profesionalizar la investigación, permitiendo no solo reaccionar, sino adelantarse a posibles ataques y comprobar hasta qué punto la organización está preparada para responder bien cuando ocurre un problema de seguridad.

---

## ¿Conocías todos los puntos tratados en la unidad? ¿Cuáles no?
Ya tenía conocimientos sobre aspectos importantes como la cadena de custodia y algunos procedimientos básicos de preservación de evidencias, porque se trata de un tema que había visto previamente en otras asignaturas. Sin embargo, reconozco que sobre MITRE ATT&CK y los diferentes marcos de respuesta a incidentes apenas había oído hablar, y no tenía claro cómo se aplicaban realmente en el entorno profesional. Gracias al trabajo realizado en clase y al estudio en profundidad del temario, he descubierto varias herramientas y técnicas que no conocía, sobre todo en lo relacionado con la preservación y el análisis de evidencias en dispositivos móviles o sistemas IOT. Me ha llamado la atención cómo se deben adaptar los procedimientos y las herramientas según el tipo de dispositivo.

---

## ¿Alguno te ha llamado especialmente la atención? ¿Por qué?
El marco RE&CT me ha resultado especialmente interesante porque está completamente orientado al ciclo de respuesta a incidentes. Su estructura por fases (preparación, identificación, contención, erradicación, recuperación, lecciones aprendidas) encaja perfectamente con escenarios reales a los que se enfrenta un equipo de seguridad. Además, la idea de visualizar el grado de madurez de una organización con “semáforos” me parece práctica y adaptable tanto en entornos grandes como en empresas más pequeñas. También me llamó la atención la importancia de la documentación y la transparencia en todos los pasos, incluso registrando lo que no se encuentra como evidencia.

---

## ¿Descartarías algún punto de la unidad? ¿Cuál y por qué?
No descartaría ningún punto. Todos los apartados me parecen muy interesantes y aportan diferentes datos para entender de mejor manera el ciclo de gestión de incidentes. Quizá algunos ejemplos podrían ser aún más prácticos para ayudar a visualizar el proceso en organizaciones con menos recursos, pero en el contexto profesional la extensión y profundidad son las adecuadas.

---

## ¿Has echado en falta algún tema?
La unidad es bastante exhaustiva en cuanto a la gestión de evidencias y el uso de marcos de investigación, pero creo que se podría ampliar algo más en la parte de herramientas concretas y aportar algún caso práctico completo, desde la detección de un incidente hasta la presentación del informe final.

---

# Resumen de la unidad

## Recopilación y almacenamiento de evidencias digitales

La gestión de evidencias digitales es uno de los pilares fundamentales en la respuesta a incidentes de ciberseguridad. Una evidencia digital puede ser desde un simple log de sistema hasta una imagen completa de disco duro, pasando por capturas de memoria, registros de red, archivos temporales, etc. Resulta esencial que el proceso de recopilación y almacenamiento garantice la integridad, autenticidad y admisibilidad de la información obtenida, ya que de ello dependerá su validez tanto a nivel técnico como legal.  
El éxito de una investigación forense depende en gran medida de la formación previa, la correcta planificación del procedimiento y la especialización del personal implicado, junto con la correcta selección de herramientas y metodologías.

La metodología más aceptada se estructura en varias etapas encadenadas: en primer lugar la **preservación** del estado original del sistema; a continuación la **adquisición** controlada de los datos relevantes; un registro meticuloso de cada intervención en la **documentación**; el posterior **análisis** objetivo del material; y, finalmente, la **presentación** clara y comprensible de los hallazgos. Todo el procedimiento debe ser transparente y reproducible, siguiendo estándares reconocidos como el RFC 3227, la UNE 71506 u otras guías internacionales.

Un punto que destaca especialmente es el criterio del **orden de volatilidad**: la prioridad debe ser extraer los datos que menos tiempo permanecen accesibles (como la RAM o las cachés) antes de recopilar información más estable (discos, logs, documentos). Al mismo tiempo, se insiste en evitar acciones que puedan modificar o invalidar la evidencia, como apagar precipitadamente el sistema o ejecutar programas potencialmente alteradores sobre el equipo comprometido. La actuación debe ser siempre proporcional y respetuosa con la privacidad, ajustándose a la legislación vigente y a las políticas internas de la organización.

## Procedimiento y cadena de custodia

El procedimiento de recopilación de evidencias es un proceso que comienza antes incluso de llegar a la escena del incidente. La **preparación** implica la comprobación de autorizaciones legales y la disposición de un kit forense adecuado (herramientas validadas, bloqueadores, medios de almacenamiento limpios, materiales de embalaje, formularios de custodia, etc.).  
En la **escena**, la prioridad es documentar exhaustivamente la situación previa a cualquier manipulación: desde esquemas y fotografías, hasta la identificación de todos los dispositivos y personas presentes. La interacción con los dispositivos debe minimizar los riesgos, empleando bloqueadores de escritura y evitando cualquier acción que pueda alterar el contenido original de los soportes digitales. La adquisición de la evidencia debe ir acompañada del cálculo de hashes antes y después de la copia, para verificar la integridad.

Al trasladar la evidencia al laboratorio, se establece el **almacenamiento seguro**: acceso restringido, protección frente a factores ambientales, uso de medios cifrados y segregados, y mantenimiento de registros de acceso a los datos. Toda manipulación o traslado queda registrada en la **cadena de custodia**, que constituye un elemento clave para asegurar la trazabilidad y validez de la evidencia en cualquier proceso judicial o auditoría interna. Al concluir el proceso, la disposición final de la evidencia (ya sea devolución o destrucción) se documenta conforme a la política y la normativa aplicable.

## Herramientas y ejemplos prácticos

Uno de los aspectos prácticos más relevantes es la correcta selección y uso de herramientas forenses. Se recomienda utilizar soluciones externas al sistema objeto de análisis para evitar posibles manipulaciones accidentales o maliciosas. Herramientas como Volatility (análisis de memoria), Wireshark (captura y análisis de tráfico de red) o ‘dd’ (imágenes “bit a bit” de discos) son ejemplos habituales en la práctica profesional. La documentación exhaustiva contiene no solo el contenido de los archivos obtenidos, sino también todos los metadatos y el contexto de la intervención.

Como ejemplo, ante un ataque DoS a un servidor web, el proceso consistiría en el aislamiento del sistema afectado, la obtención de imágenes de memoria y disco, la captura de tráfico de red relevante y el almacenamiento seguro de todo el material, incluyendo un registro estricto de la cadena de custodia.

## Marcos de investigación: MITRE ATT&CK y RE&CT

En un contexto profesional, la investigación sistemática de incidentes requiere apoyarse en marcos normalizados. En esta unidad se destaca especialmente el uso de **MITRE ATT&CK** y **RE&CT**, dos frameworks internacionales que facilitan tanto la comprensión del ciclo completo de un ataque como el diseño y evaluación de la respuesta defensiva.

MITRE ATT&CK es una base de datos estructurada alrededor de tácticas (objetivos o fines de cada fase del ataque), técnicas (cómo se logran esos objetivos), grupos de amenazas (APT) y el software que emplean. Su gran valor reside en ofrecer un lenguaje común y una visión integral de las estrategias y procedimientos empleados por los atacantes, permitiendo a analistas y equipos de respuesta anticipar, detectar y mitigar con mayor eficacia. Además, facilita la creación de matrices interactivas enfocadas en los riesgos específicos de cada sector o infraestructura.

Por su parte, RE&CT, derivado de ATT&CK, centra su estructura en el ciclo concreto de la **respuesta a incidentes**. Divide el proceso en fases claras (preparación, identificación, contención, erradicación, recuperación y lecciones aprendidas), proporcionando para cada una acciones sugeridas, técnicas recomendadas y elementos a revisar. Permite visualizar de forma rápida el grado de preparación o madurez de una organización en cada etapa, identificar áreas de mejora y documentar la gestión real de los incidentes con un enfoque práctico y dinámico.

A continuación se muestra una tabla comparativa de ambos marcos para entender mejor su aplicación:

| Marco           | Enfoque principal                       | Elementos clave                | Utilidad principal                   |
| --------------- | -------------------------------------- | ------------------------------ | ------------------------------------ |
| MITRE ATT&CK    | Identificación y análisis de amenazas  | Tácticas, técnicas, grupos APT, software, mitigaciones | Inteligencia, detección, análisis, formación, evaluación de seguridad |
| RE&CT           | Respuesta a incidentes (DFIR)          | Fases (preparación, identificación, etc.), acciones de respuesta | Guía de respuesta, medición de madurez, documentación, playbooks      |

Ambos marcos, correctamente aplicados, no solo ayudan a sistematizar la labor de los equipos de ciberseguridad (blue/red team), sino que también sirven como referencia para la formación continua, la automatización de respuestas y la mejora constante de los procesos internos.

## Conclusiones

En definitiva, la unidad proporciona una visión práctica, actualizada y profundamente profesional de la gestión de incidentes de ciberseguridad, con especial énfasis en la recolección, almacenamiento y uso estratégico de evidencias digitales. Además, pone sobre la mesa la integración de marcos internacionales que facilitan la mejora continua, la colaboración entre equipos y la defensa proactiva frente a amenazas cada vez más sofisticadas.  
El dominio de estos procedimientos, así como el uso inteligente de las herramientas y marcos estudiados, resulta esencial para cualquier organización que aspire a una seguridad robusta y a una gestión eficiente de sus incidentes.