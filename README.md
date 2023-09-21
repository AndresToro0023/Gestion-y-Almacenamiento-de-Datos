# Proyecto Final - Analisis Consumo Energetico Horario MWh
@Reyesbt21
@LuisFernandoZuluaga

## Problematica
PJM Interconnection LLC (PJM), es una organización de transmisión de energía de la región oriental que estados unidos y que tiene incidencia en todo o partes de Delaware, Illinois, Indiana, Kentucky, Maryland, Michigan, Nueva Jersey, Carolina del Norte, Ohio, Pensilvania, Tennessee, Virginia, Virginia Occidental y el Distrito de Columbia. 
Con el análisis de los consumos(en Megavatios) se podría predecir como seria la demanda de energía que se requiere por cada franja horaria permitiendo a los entes que generan la energía poder hacer proyecciones de la cantidad de energía que deben tener disponible en cada franja horaria.

## Contenido del Repositorio
En el repositorio se encuentra la base de informacion de consumo energetico en MWh para estados de USA, adicional se encuentra el scip con el cual se realiza el analisis y estructuracion de los datos, el cual reemplaza los datos nulos por consumos promedios de acuerdo a las franjas horarias, como resultado del scrip anterior se anexa eñ la base de datos completa sin valores nulos.
Por ultimo se incluye scrip en el cual por medio de sqlite3 se realiza manipulacion de la base de datos final (Creacion de base de datos, ingreso de informacion, consultas y eliminacion )

## Cuantos datos tomó, de que son y cuantas características tienen
Inicialmente contamos con 2.317.406 datos del consumo energetico en MWh en 13 características y 178262 registros:
1. Datetime
2. AEP
3. COMED
4. DAYTON
5. DEOK
6. DOM
7. DUQ
8. EKPC
9. FE
10. NI
11. PJME
12. PJMW
13. PJM_Load

## Que encontró en los datos
Como resultado del proceso de analisis y trasnformacion de la informacion, encontramos mediciones de consumos energetico de forma individual para cada uno de los estados en cuatro diferentes tiempos, anuales, mensuales, diarios y horarios, de esta forma se identifican patrones de comportamiento de consumo con diferencias en cada tiempo y cada estado.

## Cómo su descubrimiento podría dar valor a una empresa
Colocar en funcionamiento un generador es costoso para los operadores de red, por esta razón el poder hacer proyecciones de respuesta a la demanda podría ayudar a los operadores de red a no incurrir en gastos innecesarios, adicionalmente podría ayudarle al operador de red a generar estrategias que le permitan allanar la curva de consumo de energía, optimizando los recursos.
Dentro las estrategias que se puede implementar, podría ser el cobro de energía por periodos tarifarios que genera valor tanto a la empresa como a los usuarios, por ejemplo, vendiendo el KWh a un precio más económico en las horas de baja demanda de energía y a un precio mayor en las franjas de mayor demanda, incentivando el ahorro de energía en las horas pico generando un aplanamiento de la curva de consumo de energía.
