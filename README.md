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

*(completar con las conclusiones una vez interpretados los resultados)*

# Cómo usar este proyecto

1. Clona el repositorio.
2. Abre `analisis_premier_league.xlsx`.
3. Usa los slicers de las tablas dinámicas para filtrar por temporada y explorar los resultados.

# Autor

Proyecto realizado como parte de una ruta de aprendizaje en análisis de datos, orientado a la construcción de portafolio para postulación a vacantes de Analista de Datos Jr.

