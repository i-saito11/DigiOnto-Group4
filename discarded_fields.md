# Justificación de Campos Descartados

Durante el análisis de las fuentes de datos originales, hemos decidido no modelar ni incluir los siguientes campos en los requisitos funcionales de nuestra ontología, por las razones de diseño que se exponen a continuación:

* **`Number` (Dataset DigiDB)**: Se descarta este campo porque es puramente un identificador numérico interno (índice). Utilizaremos el nombre de la criatura (Digimon) como identificador único.
* **`Equip Slots` (Dataset DigiDB)**:  Indica cuántos objetos puede equiparse un Digimon. Se ha descartado porque nuestra ontología se centra en características intrínsecas, dejando fuera mecánicas de inventario.
* **`Memory` (Dataset DigiDB)**: Se descarta por su ambigüedad semántica fuera del contexto del videojuego. Representa un coste artificial de balanceo de equipo que no aporta valor a las características reales de la criatura.
* **`Power`y`Categoría Física/Mágica` (Dataset Movelist)**:Por decisión de diseño (Scoping), el modelado de habilidades se ha restringido **únicamente a los movimientos de soporte (Support)**. Dado que las habilidades de soporte no causan daño directo, los campos de poder de ataque y su categoría de daño carecen de sentido en esta ontología y han sido descartados.
