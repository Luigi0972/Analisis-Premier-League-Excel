# Análisis Premier League – Excel Avanzado

Proyecto de portafolio de análisis de datos. Analiza las últimas 5 temporadas de la Premier League usando Excel avanzado: Power Query, tablas dinámicas y gráficos dinámicos.

# Objetivo

Explorar el rendimiento de los equipos de la Premier League a lo largo de 5 temporadas, evaluando resultados, disciplina (tarjetas) y diferencias de rendimiento entre condición local y visitante.

# Herramientas

- Excel (Power Query, Tablas dinámicas, Gráficos dinámicos)
- Fuente de datos: archivos CSV con resultados de partidos de las últimas 5 temporadas de la Premier League

# Estructura del repositorio

analisis-premier-league-excel/
├── data/
│ └── (archivos CSV originales por temporada)
├── analisis_premier_league.xlsx
└── README.md


# Proceso (Power Query)

1. **Carga de datos**: importación de los CSV de las 5 temporadas.
2. **Transformación**: construcción de la tabla `BaseEquipos`, combinando las vistas Local y Visitante en una sola fila por equipo por partido.
3. **Columnas auxiliares**: creación de los campos `Victoria` y `PartidoJugado` para poder calcular porcentajes de victorias por condición (local/visitante).

# Análisis realizados

| # | Análisis | Tipo de visual | Filtro |
|---|----------|-----------------|--------|
| 1 | Ranking de equipos: Goles a Favor, Goles en Contra, Tarjetas Amarillas y Rojas | Tabla y gráfico dinámico | Slicer de Temporada |
| 2 | % de Victorias Local vs. Visitante por equipo | Tabla y gráfico dinámico (campo calculado) | — |

# Principales hallazgos

No se encontró una relación clara entre la indisciplina de un equipo (tarjetas amarillas y rojas) y su rendimiento (diferencia de goles). Equipos con muchas tarjetas, como Chelsea y Manchester United, tuvieron diferencia de goles positiva, mientras que otros con niveles similares de tarjetas, como Wolves y Everton, tuvieron diferencia de goles muy negativa. Esto sugiere que la indisciplina por sí sola no es un buen predictor del rendimiento de un equipo.

También se observó que los equipos recién ascendidos o con menos temporadas en la liga (Luton, Sunderland, Ipswich, Sheffield United, Watford, Norwich) muestran totales de goles y tarjetas mucho más bajos — no porque sean más disciplinados o defensivos, sino porque jugaron menos partidos en el periodo analizado. Para futuras versiones de este análisis, sería útil normalizar estas métricas por partidos jugados antes de comparar equipos.

# Cómo usar este proyecto

1. Clona el repositorio.
2. Abre `analisis_premier_league.xlsx`.
3. Usa los slicers de las tablas dinámicas para filtrar por temporada y explorar los resultados.

# Autor

Proyecto realizado como parte de una ruta de aprendizaje en análisis de datos, orientado a la construcción de portafolio para postulación a vacantes de Analista de Datos Jr.

