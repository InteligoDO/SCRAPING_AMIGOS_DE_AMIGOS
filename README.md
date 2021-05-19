# Scrapping amigos de amigos (olas)

El proceso consiste en conocer los amigos de las personas procesadas en el SP de adquisición, estos amigos pueden ser: clientes, apóstoles, potencial medio, potencial alo y potencial muy alto.

Este proceso, se ha dividio en 3 partes:

## Primero - Obtener las personas a scrapear por ola

Para obtener las personas a scrapear en la ola actual se debe ejecutar el archivo **Persons_to_scrap.ipynb**.

En este paso, tener en cuenta que se debe guardar en un excel la información del SP que completa el área de adquisición.

Para que la información del SP incluya la información de los DNIs últimos, se debe hacer un previo aviso a Adquisición (Paolo).

## Segundo - Scraping

Para realizar el scraping se debe ejecutar el archivo **scrappingloop.ipynb**

Este archivo necesita ser ejecutado una vez al día, y se debe actualizar diariamente la variable *targets_5* ya que define las 5 personas que se van a scrapear en ese día.

## Tercero - Agregar información actualizada a DB de adquisición

En este último paso se debe ejecutar el archivo **update_ADQ_AMIGOS_DE_PROSPECTOS.ipynb** que transforma y ordenar la información del SP con lo obtenido en el scraping de todas las olas realizadas.

Tener en cuenta que se debe escribir el nombre de la persona que está realizando el scraping en la variable *usuario*, esta información es necesaria al momento de actualizar la información en la base de datos.





