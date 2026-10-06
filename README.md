# Base Única de Instituciones Educativas (B.U.D.I.E.) · Río Cuarto

El dashboard **B.U.D.I.E.** centraliza y georreferencia la oferta educativa de Río Cuarto en un visor interactivo. Permite consultar matrículas, niveles, sectores, accesibilidad física y datos de contacto, con filtros avanzados, sincronización en vivo con la base oficial y un mapa territorial basado en capas del IGN.

---

## 🚀 Características Principales

- **Tablero Interactivo de Indicadores**: Estadísticas consolidadas de instituciones, matrícula, modalidades, sectores de gestión y niveles educativos.
- **Georreferenciación Territorial con Cartografía Oficial**: Integración con capas base del **Instituto Geográfico Nacional (IGN Argentina)** y división barrial de Río Cuarto en formato GeoJSON.
- **Sincronización en Vivo**: Botón de actualización en tiempo real que consulta la planilla oficial en Google Sheets vía API GViz con fallback JSONP (apto tanto para despliegues web como para ejecución local `file:///`).
- **Indicadores de Accesibilidad y Contacto en Alto Contraste**: Diferenciación visual inmediata mediante colores institucionales:
  - 🟢 **Verde**: Atributo presente / disponible.
  - 🔴 **Rojo**: Atributo no disponible / sin dato.
- **Búsqueda Inteligente**: Búsqueda multi-token y normalizada por nombre, CUE, barrio, calle, directivos y alias institucionales.
- **Fichas Técnicas Individuales**: Modales interactivos y panel lateral en el mapa con información detallada por establecimiento.

---

## 📁 Estructura del Proyecto

```
├── Dashboard Instituciones Educativas - BUDIE.html   # Tablero principal de visualización y tabla interactiva
├── mapa.html                                        # Visor cartográfico territorial con Leaflet + IGN
├── index.html                                       # Redirección automática al tablero principal
├── assets/                                          # Recursos gráficos (logos institucionales, ODS) y GeoJSON de barrios
│   ├── barrios_geojson.js
│   ├── rio-cuarto-vos.png
│   ├── datos-rio-cuarto.png
│   └── ...
└── README.md
```

---

## 🛠️ Tecnologías Utilizadas

- **HTML5 / CSS3** (Diseño responsivo basado en tokens institucionales de Río Cuarto y Obelisco)
- **Vanilla JavaScript (ES6+)**
- **Leaflet.js** (Visor cartográfico)
- **IGN Argentina / Argenmap** (Capas de mapas base)
- **Google Sheets GViz API** (Sincronización de base de datos)

---

## 🏛️ Gobierno de Río Cuarto
**Dirección de Estadística · Secretaría de Gobierno y Participación Ciudadana**
