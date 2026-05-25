# Calculadora de Crédito Hipotecario

Herramienta personal para simular y comparar créditos hipotecarios en pesos colombianos (COP). Funciona 100% en el navegador, sin backend ni dependencias de build.

🔗 **[Abrir calculadora](https://TU_USUARIO.github.io/TU_REPOSITORIO/)**

---

## Funcionalidades

- **Sistema francés** (cuota fija) con conversión de tasa efectiva anual a mensual
- **Comparador de dos tasas** en paralelo con diferencias de cuota y costo total
- **Seguros mensuales** (vida, incendio, otro) configurables como % del saldo o monto fijo
- **Abonos extra** a capital: únicos, desde una cuota, o cada 12 meses
- **Gráficas** de evolución de saldo y composición capital/interés (Chart.js)
- **Resumen comparativo** con plazo efectivo, intereses y ahorro por abonos
- **Tabla de amortización** mes a mes con exportación a CSV y PDF
- Soporte automático de **modo oscuro**

## Uso

Abre directamente `index.html` en el navegador con doble clic — no requiere servidor, npm ni ningún paso de build.

## Stack

| Tecnología | Uso |
|---|---|
| HTML + CSS + JS vanilla | Todo el frontend y lógica |
| [Chart.js 4.4.1](https://www.chartjs.org/) | Gráficas (cargado por CDN) |

## Fórmulas financieras

**Cuota fija (sistema francés):**
```
C = P × [ i × (1+i)^n ] / [ (1+i)^n − 1 ]
```

**Conversión tasa anual efectiva → mensual:**
```
i_mensual = (1 + i_anual)^(1/12) − 1
```

## Publicar en GitHub Pages

1. Sube este repositorio a GitHub
2. Ve a **Settings → Pages**
3. En *Source* selecciona la rama `main` y carpeta `/ (root)`
4. Guarda — en unos segundos tendrás la URL pública

## Licencia

Uso personal. Sin licencia de distribución.
