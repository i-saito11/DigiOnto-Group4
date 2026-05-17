# DigiOnto: Ontology Requirements Specification 

[![v1.0.0](https://img.shields.io/badge/docs-v1.0.0-blue)](https://i-saito11.github.io/Digionto-Group4/1.0.0/index-en.html) [![v1.0.1](https://img.shields.io/badge/docs-v1.0.1-green)](https://i-saito11.github.io/Digionto-Group4/1.0.1/index-en.html)

Bienvenidos al repositorio oficial del **Grupo 4** para la práctica de Especificación de Requisitos Ontológicos. 

Este proyecto define los requisitos funcionales y no funcionales para la creación de **DigiOnto**, una ontología semántica diseñada para modelar el ecosistema de criaturas digitales (Digimon), sus líneas evolutivas y mecánicas de combate.

## Estructura del Repositorio

El proyecto ha evolucionado y ahora se estructura en base a sus **versiones**. En la raíz del repositorio encontraréis las carpetas de las versiones publicadas (**`1.0.0/`** y **`1.0.1/`**). 

Dentro de cada carpeta de versión se incluye el conjunto completo de artefactos y documentación:

* **Documentación Web (Widoco)**: Archivos HTML estáticos, siendo `index-en.html` la página principal generada a partir de la ontología.
* **Ontología (`ontology.*` y `ontologia_def_*`)**: El código fuente de la ontología disponible en múltiples formatos de serialización (OWL/XML, Turtle, N-Triples, JSON-LD).
* **`.htaccess`**: Archivo de configuración que habilita la *Negociación de Contenido* en GitHub Pages para servir el formato adecuado según la petición del cliente.
* **Documentación Técnica**:
  * **`OntologyRequirements_Updated.csv`**: Archivo principal que contiene los requisitos funcionales formateados como Preguntas de Competencia (Competency Questions).
  * **`use_cases.md`**: Casos de uso principales (Team Builder competitivo y Enciclopedia Semántica) que motivan el desarrollo.
  * **`discarded_fields.md`**: Justificación técnica de las variables excluidas del modelado conceptual.
  * **`datasets_links.md`**: Referencias y enlaces a los datasets utilizados.
* **Diagramas**: Diseños conceptuales siguiendo la nomenclatura Chowlk. Cada versión incluye los archivos fuente editables (`.drawio`) y su exportación para visualización (`.pdf`). En la versión `1.0.1` se encuentran los diagramas definitivos.
* **`shacl/`**: Carpeta destinada a la validación de la ontología mediante Shapes Constraint Language:
  * **`shapes.ttl`** / **`shape.ttl`**: Definición de las restricciones estructurales (Filtro de calidad) basadas en los requisitos.
  * **`data.ttl`**: Instancias de prueba del dominio Digimon (válidas y con errores inyectados).
  * **`report.ttl`**: Informe generado que documenta el cumplimiento o las violaciones de las reglas.

## Fuentes de Datos

La ontología se basa en la integración de las siguientes fuentes:
1. **Dataset Principal asignado**: [DigiDB - Digimon Database](https://www.kaggle.com/datasets/rtatman/digidb) (Estadísticas base, atributos y tipos).
2. **Dataset Adicional (Extensión del dominio)**: [DigiDB Support Movelist](https://www.kaggle.com/datasets/rtatman/digidb?select=DigiDB_supportlist.csv) (Ataques de support).
3. **Dataset Adicional (Extensión del dominio)**: [DigiDB Movelist](https://www.kaggle.com/datasets/rtatman/digidb?select=DigiDB_movelist.csv) (Listado de ataques). Utilizando la sugerencia de clase hemos añadido este dataset pues, necesitamos más datos.

## Autores - Grupo 4
* Miguel Díaz Martín
* Íñigo Rodríguez Saito
* Andrés Knyshayid Voronovskyy
* José Gómez Monjo

---
*Práctica desarrollada para la asignatura de Developing Open, Interoperable Semantic Resources.*
