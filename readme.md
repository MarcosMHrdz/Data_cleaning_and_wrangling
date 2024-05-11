![logo_ironhack_blue 7](https://user-images.githubusercontent.com/23629340/40541063-a07a0a8a-601a-11e8-91b5-2f13e4e6b441.png)

# Laboratorio | Limpieza y discusión de datos.

Para esta práctica de laboratorio, usaremos el mismo conjunto de datos que usamos en las prácticas de laboratorio anteriores. Recomendamos usar el mismo cuaderno, ya que reutilizará las mismas variables que creó y usó anteriormente en los laboratorios.

### Instrucciones

Hasta ahora hemos trabajado en "EDA". Esta práctica de laboratorio se centrará en la limpieza y discusión de datos de todo lo que notamos antes.

1. Comenzaremos eliminando los valores atípicos. Hasta ahora, hemos analizado diferentes métodos para eliminar valores atípicos. Utilice el que le resulte más cómodo y defina una función para ello. Utilice la función para eliminar los valores atípicos y aplicarlos al marco de datos.
2. Cree una copia del marco de datos para la manipulación de datos.
3. Normalizar las variables continuas. Puede utilizar cualquier método que desee.
4. Codifique las variables categóricas.
5. La variable tiempo puede resultar útil. Intente transformar sus datos en datos útiles. Sugerencia: Puede resultar útil utilizar el día, la semana y el mes como números enteros.
6. Dado que el modelo solo aceptará datos numéricos, verifique y asegúrese de que cada columna sea numérica; si algunas no lo son, cámbielas mediante codificación.

**Sugerencia para variables categóricas**

- Debes tratar con las variables categóricas como se muestra a continuación (para la codificación ordinal, también se ha proporcionado un código ficticio):

```pitón
# Uno caliente para declarar
# Ordinal a la cobertura
# Ordinal al estado laboral
# Ordinal al código de ubicación
# Uno caliente al estado civil
# Un tipo de política atractivo
# Uno caliente para la política
# Una oferta interesante para renovarcustomer_df
# Un canal atractivo para las ventas
# Una clase de vehículo caliente
# Tamaño normal del vehículo

datos["cobertura"] = datos["cobertura"].map({"Básico": 0, "Extendido": 1, "Premium": 2})
# dado que la columna "cobertura" en el marco de datos "datos" tiene tres categorías:
# "básico", "extendido" y "premium" y los valores deben representarse en el mismo orden.
```