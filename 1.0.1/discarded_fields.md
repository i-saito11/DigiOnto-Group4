# Justificación de Campos Descartados

Durante el análisis de las fuentes de datos originales, hemos decidido no modelar ni incluir los siguientes campos en los requisitos funcionales de nuestra ontología, por las razones de diseño que se exponen a continuación:

* **`Number` (Dataset DigiDB)**: Se descarta este campo porque es puramente un identificador numérico interno (índice). Utilizaremos el nombre de la criatura (Digimon) como identificador único.
* **`Equip Slots` (Dataset DigiDB)**:  Indica cuántos objetos puede equiparse un Digimon. Se ha descartado porque nuestra ontología se centra en características intrínsecas, dejando fuera mecánicas de inventario.

* **`Inheritable` (Dataset DigiDB)**: Indica si una habilidad puede ser transferida entre diferentes criaturas a través de la evolución. Se descarta porque representa una mecánica de progresión y herencia propia del sistema de juego, mientras que nuestra ontología se enfoca en las características esenciales de los Digimon y los atributos de combate de los movimientos de forma independiente. 
