## Proyecto: Dashboard Financiero — Mercado Pago Servicios de Procesamiento S.R.L.

### Descripción de la Empresa

Mercado Pago Servicios de Procesamiento S.R.L. es una sociedad constituida en Argentina en agosto de 2020, controlada en un 95% por MercadoPago LLC, la cual a su vez pertenece al grupo MercadoLibre Inc. La compañía opera principalmente como **adquirente** dentro del ecosistema de medios de pago electrónicos, procesando transacciones con tarjetas de crédito, débito, comerciales y prepagas para comercios adheridos. A partir de julio de 2025 incorporó un nuevo segmento de servicios financieros consistente en el **adelanto de cupones de ventas en cuotas** a comercios, instrumentado con recurso. Sus estados financieros al 31 de diciembre de 2025 fueron preparados por primera vez bajo Normas de Contabilidad NIIF, auditados por Ernst & Young (EY), y presentados ante la Comisión Nacional de Valores (CNV) en el marco de la emisión de obligaciones negociables simples por hasta USD 500.000.000.

Puede visualizar y utilizar el reporte creado en este link: https://lnkd.in/db69RFzw

---

### Objetivo del Proyecto

El objetivo principal de este proyecto fue desarrollar un **reporte financiero interactivo en Power BI** que permita analizar en profundidad la situación patrimonial, económica y financiera de Mercado Pago Servicios de Procesamiento S.R.L., tomando como base sus estados financieros comparativos al 31 de diciembre de 2025 y 2024. El reporte está orientado a facilitar la toma de decisiones mediante visualizaciones claras y métricas financieras relevantes, considerando las particularidades del modelo de negocio de adquirencia y el contexto macroeconómico argentino de alta inflación bajo el cual fueron preparados los estados financieros.

---

### Desarrollo del Proyecto

El desarrollo del reporte comprendió las siguientes etapas:

**Extracción y transformación de datos con Python**
Los datos fueron extraídos directamente de los estados financieros auditados e integrados al modelo mediante un proceso de limpieza y estructuración desarrollado en Python utilizando la librería **pandas**. Este proceso incluyó la construcción de tablas de dimensiones, la asignación de identificadores numéricos por cuenta contable, la construcción de una tabla calendario con locale en español y la definición de la jerarquía de categorías (Activo, Pasivo, Patrimonio) y subcategorías necesarias para el correcto funcionamiento del modelo semántico en Power BI.

**Modelado y medidas DAX**
Se desarrollaron **130 medidas DAX** que cubren los distintos ejes del análisis financiero. Entre las medidas de mayor relevancia presentes en el overview del reporte se destacan:

- **SCC** (Suficiencia de capital corriente) — Determinacion del capital corriente sobre el capital corriente operativo
- **RE** (Rentabilidad Economica) — Eficiencia en el uso de los activos
- **RF** (NRentabilidad Financiera) — Medida de rentabilidad del capital propio sin considerar efecto de impuesto o resultados extraordinarios
- **Efecto Palanca** — El leverage de la rentabilidad por la utilizacion de capitales de terceros
- **Análisis Vertical** — Participación porcentual de cada cuenta sobre el total del activo y sobre el total del pasivo más patrimonio
- **Variación interanual (%)** — Comparación de cada rubro entre ejercicios con tratamiento correcto de bases negativas
- **Resultado Operativo / EBIT** — Aislando resultados no operativos como RECPAM y diferencia de cambio
- **Ratios de liquidez y solvencia** — Liquidez corriente, ratio de endeudamiento y cobertura de capital

**Diseño del background en Figma**
El diseño visual del reporte fue desarrollado íntegramente en **Figma**, donde se construyó el background personalizado de cada página del dashboard. El diseño contempla una identidad visual coherente con el perfil corporativo financiero del reporte, optimizando la disposición de los elementos visuales, la paleta de colores y la tipografía para garantizar legibilidad y una experiencia de usuario profesional dentro del entorno de Power BI.

---

### Consideraciones del Análisis

El análisis contempla las particularidades contables y de negocio propias de la compañía, entre ellas la aplicación de la **NIC 29** (economía hiperinflacionaria) con cifras expresadas en moneda homogénea al 31 de diciembre de 2025, la distinción entre el segmento de adquirencia y el nuevo segmento de otros servicios financieros, el tratamiento del **RECPAM** como resultado no operativo a los efectos del análisis de performance, y la naturaleza de los créditos con entidades de cobro como activos de intermediación que no conllevan riesgo crediticio directo para la sociedad según lo establecido por su propia gerencia y validado por los auditores externos.

---

### Stack Tecnológico

| Herramienta | Uso |
|---|---|
| **Python / pandas** | Extracción, limpieza y estructuración de datos |
| **Power BI** | Modelado semántico, visualización e interactividad |
| **DAX** | 130 medidas para análisis financiero |
| **Figma** | Diseño del background y layout del reporte |

---

### Desarrollo del reporte

Semnalmente publico en LinkedIn de manera desglosada la preparacion, desarrollo y terminacion del reporte en cuestion. 
Para ver mas detalles mi Linkedin es: www.linkedin.com/in/victoria-luz-pereyra-03b63b173
