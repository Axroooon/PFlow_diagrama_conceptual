# PFlow - Diagrama Conceptual (Modelo de Chen)

Este directorio contiene el diagrama conceptual de la base de datos de PFlow utilizando la notación de Peter Chen. Su objetivo es modelar las entidades, atributos y relaciones lógicas del flujo de atención en emergencias hospitalarias de manera independiente al motor de base de datos relacional final.

## Estructura del Diagrama

* **Entidades (Rectángulos):** 11 entidades principales que representan el modelo de negocio (EstablecimientoSalud, Paciente, AtencionEmergencia, EventoAtencion, etc.).
* **Atributos (Óvalos):** Propiedades atómicas de cada entidad. Las llaves primarias están identificadas explícitamente. No se incluyen llaves foráneas como atributos, ya que estas se representan a través de las conexiones lógicas.
* **Relaciones (Rombos):** Verbos lógicos que conectan las entidades (ej. "recibe", "registra", "involucra"). 
* **Cardinalidad:** Definida en los conectores (1 a N, 1 a 1). El modelo está diseñado sin relaciones de muchos a muchos (N:M) gracias a la normalización mediante las entidades transaccionales `AtencionEmergencia` y `EventoAtencion`.

## Archivos Incluidos

* `modelo_logico_chen.drawio`: Archivo fuente editable del diagrama.
* `modelo_logico_chen.png`: Exportación gráfica con fondo sólido para incluir en el informe del proyecto final.

## Herramientas de Edición

Para visualizar o modificar el archivo `.drawio`, puedes utilizar cualquiera de las siguientes opciones:
1. La aplicación web o de escritorio gratuita [diagrams.net (draw.io)](https://app.diagrams.net/).
2. Visual Studio Code instalando la extensión oficial **Draw.io Integration**.