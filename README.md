# Radiografía de la informalidad laboral en Colombia año 2022
# Descripción y motivación

Estamos en vísperas del inicio de la negociación del salario mínimo para 2023, y, una vez más, se excluye al sector informal. Pese a la evidencia y advertencias sobre los efectos de la regulación en la informalidad, es una situación que se repite cada año. Por otro lado, no se dimensiona que la informalidad laboral afecta otros sectores por la ausencia de contribuciones al sistema de seguridad social. Y, al mismo tiempo, el sistema contributivo de seguridad social genera mayores costos a la contratación formal. Por otra parte, hace 5 años Colombia hace parte de la OCDE, y uno de sus peores indicadores con respecto a los miembros es la informalidad, destacando, además, que sus regulaciones en materia laboral están en las antípodas de las adoptadas por los países con menores tasas de informalidad.
Así pues, este trabajo busca dimensionar la informalidad; identificarla, clasificarla y diferenciarla. Pues, entre mejor se diagnostica, cuantifica y entiende un problema público, mayor éxito tendrán las políticas implementadas. Por otro lado, soy férrea defensora de las políticas públicas que se focalizan en subgrupos poblacionales, entendiendo que no todas las dinámicas y necesidades son iguales.
Así pues, con el fin de conocer de qué manera y a quiénes impacta la informalidad, en este proyecto se buscó sacar las estadísticas por subgrupos poblacionales de interés, así como buscar los efectos que tiene pertenecer a un grupo en la probabilidad de ser informal.

Algunas hipótesis-preguntas que me motivaron:
*¿qué sucede en los departamentos con mayor informalidad?
*En este sector existe una brecha de género significativa?
*Cómo se distribuye la informalidad entre las minorías?
*qué políticas toman los países desarrollados para tener cifras de informalidad considerablemente menores que Colombia?

# métodos usados

1. procesamiento y análisis exploratorio de datos con la librería pandas y numpy para limpieza de la Gran Encuesta Integrada de Hogares 2022 y bases OCDE 2021.
2. regresión logística con la librería statsmodels apartir de unas variables de interés como el sexo, etnia y nivel educativo.
3. creación de dataframes filtrados con pandas para realizar cálculos y posteriormente hacer visualizaciones gráficas.
4. Visualización de datos con matplotlib y seaborn, implementando principalmente gráficos de barras.
5. Exportar los gráficos y utilizarlos en un notebook donde se compactan los resultados del análisis exploratorio y datos y sus interpretaciones.

# Metodología
En un notebook llamado Procesamiento GEIH2022 se realizó toda la limpieza de la GEIH, y en el que se calculó la informalidad apartir de las definiciones del DANE con una estructura de condiciones para crear otra variable dummy. EL Dataframe procesado se utiliza en un siguiente notebook llamado EDA GEIH 2022 y OCDE2021, en el cual se realizaron cálculos de estadísticas de resumen y ponderaciones para empezar delimitar la informalidad por subgrupos. De igual forma, en este notebook se procesaron bases de la OCDE para computarlas en una sola. Todos los dataframes creados en ese notebook fueron exportados en csv. En un tercer notebook llamado Modelo logit se llevó acabo el modelo. En un cuarto notebook llamado DataViz se realizaron todos los gráficos apartir de las bases creadas en el notebook 2. Por último, en un notebook que lleva el título de este proyecto se hicieron las interpretaciones en markdowns y se adjuntaron todas las gráficas.


# Principales hallazgos
*En los departamentos con mayor informalidad el salario mínimo es significativamente más alto que el salario promedio. 
*Los hombres se encuentran más en el sector informal que las mujeres.
*La informalidad de los Indígenas, afros y mulatos es mayor que en aquellas personas que no se identifican con una etnia.
*A mayor nivel educativo, menor probabilidad de informalidad.

# Referencias:
Histórico del salario mínimo en Colombia. (s. f.). https://www.salariominimocolombia.net/historico/
DANE(2022). Gran Encuesta Integrada de Hogares - GEIH - 2022. https://microdatos.dane.gov.co/index.php/catalog/771/data-dictionary/F56?file_name=Ocupados
OECD(s.f) - Tax on Corporate Profits - OECD data. theOECD. https://data.oecd.org/tax/tax-on-corporate-profits.htm
PNUD(2021). Mercados laborales fragmentados.
