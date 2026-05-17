# DigiOnto: Ontology Requirements Specification 

[![v1.0.0](https://img.shields.io/badge/docs-v1.0.0-blue)](https://i-saito11.github.io/DigiOnto-Group4/1.0.0/index-en.html)

[![v1.0.1](https://img.shields.io/badge/docs-v1.0.1-green)](https://i-saito11.github.io/DigiOnto-Group4/1.0.1/index-en.html)

Bienvenidos al repositorio oficial del **Grupo 4** para la práctica de Especificación de Requisitos Ontológicos. 

Este proyecto define los requisitos funcionales y no funcionales para la creación de **DigiOnto**, una ontología semántica diseñada para modelar el ecosistema de criaturas digitales (Digimon), sus líneas evolutivas y mecánicas de combate.

## Estructura del Repositorio

Para cumplir con los criterios de evaluación de la asignatura, este repositorio contiene los siguientes entregables:

*  **`OntologyRequirements_Updated.csv`**: Archivo principal que contiene los 20 requisitos funcionales formateados como Preguntas de Competencia (Competency Questions).

*  **`use_cases.md`**: Documento que detalla los 2 casos de uso principales (Team Builder competitivo y Enciclopedia Semántica) que motivan el desarrollo de esta ontología.

*  **`discarded_fields.md`**: Justificación técnica de las variables y columnas de los datasets originales que han sido excluidas del modelado conceptual.

*  **`datasets_links.md`**: Referencias y enlaces a los datasets utilizados (DigiDB principal y Movelist extendido) extraídos de Kaggle.

* **`diagramas/`**: Carpeta que contiene los diagramas conceptuales siguiendo nomenclatura Chowlk. Se incluyen dos diseños, cada una con su archivo fuente editable (`.drawio`) y su versión exportada para fácil visualización (`.pdf`):
  * **Diagrama Inicial**: Primer borrador del modelo conceptual (`diagrama_inicial.drawio` y `Chowlk_Developing.drawio.pdf`).
  * **Diagrama Corregido**: Versión final refinada tras aplicar las correcciones pertinentes (`diagrama_corregido.drawio` y `diagrama_corregido.drawio.pdf`).
 
 * **`shacl/`**: Carpeta destinada a la validación de la ontología mediante Shapes Constraint Language:
    * **shapes.ttl**: Definición de las restricciones estructurales (Filtro de calidad) en lenguaje SHACL basadas en nuestros requisitos funcionales.
    * **data.ttl**: Instancias de prueba del dominio Digimon (tanto válidas como con errores inyectados a propósito) para evaluar las reglas.
    * **report.ttl**: Informe de validación generado que documenta qué datos cumplen con las reglas definidas y qué violaciones se han detectado.

##  Fuentes de Datos

La ontología se basa en la integración de las siguientes fuentes:
1. **Dataset Principal asignado**: [DigiDB - Digimon Database](https://www.kaggle.com/datasets/rtatman/digidb) (Estadísticas base, atributos y tipos).
2. **Dataset Adicional (Extensión del dominio)**: [DigiDB Support Movelist](https://www.kaggle.com/datasets/rtatman/digidb?select=DigiDB_supportlist.csv) (Ataques de support).
3. **Dataset Adicional (Extensión del dominio)**: [DigiDB Movelist](https://www.kaggle.com/datasets/rtatman/digidb?select=DigiDB_movelist.csv) (Listado de ataques). Utilizando la sugerencia de clase hemos añadido este dataset pues, necesitamos más datos.

##  Autores - Grupo 4
* Miguel Díaz Martín
* Íñigo Rodríguez Saito
* Andrés Knyshayid Voronovskyy
* José Gómez Monjo

---
*Práctica desarrollada para la asignatura de Developing Open, Interoperable Semantic Resources.*

