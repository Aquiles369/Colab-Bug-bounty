# v0.1 — 2025-10-03

**TL;DR:** Primera release pública — panel web ligero para gestión colaborativa de reports de bug bounty. Interfaz local (HTML/JS) con CRUD, buscador por ID, selección múltiple, export/import (JSON/CSV) y persistencia en `localStorage`. Ideal para labs y para organizar triage y pagos sin dependencias externas.

✅ **Incluye**
- Interfaz `.html` lista para usar (offline, guardado en localStorage).  
- Buscador por ID de informe y edición CRUD (añadir/editar/borrar filas y columnas).  
- Selección múltiple con casillas (editar/borrar en lote).  
- Export / Import en JSON y CSV (compartir con colegas).  
- Indicador visual en Notas (círculo rojo si hay contenido).  
- Estados coloreados para severidad y triage.  
- Tabla principal con 10 columnas predefinidas (ver README).  
- Persistencia local: todo se guarda en `localStorage` (offline).  
- Demo GIF + walkthrough disponible en README / carpeta `assets`.

🛠️ **Quickstart**
```bash
# clonar
git clone https://github.com/Aquiles369/<REPO>.git
cd <REPO>/web   # o la carpeta donde esté tools.html

# opción 1: abrir directamente (sin servidor)
# doble click en tools.html o:
xdg-open tools.html   # linux
open tools.html       # macOS
start tools.html      # Windows

# opción 2 (recomendado, evita problemas con fetch/XHR)
python3 -m http.server 8000
# abrir en: http://127.0.0.1:8000/tools.html


⚠️ Notas de seguridad / uso

Esta herramienta guarda datos en localStorage del navegador. No almacenes información sensible en repositorios públicos.

Uso sólo en entornos permitidos: no usar para targets sin permiso. PoC / demos marcadas lab-only.

Si vas a compartir datos entre colegas, exporta a JSON/CSV y comparte el archivo, no la instancia local del navegador.

📄 Formato de columnas (predeterminado)

Título del reporte

ID de informe

Fecha de reporte

Encontrado por

Reportado por

Severidad / Estado

Triage / Estado de gestión

Bounty — quien cobró

Bounty — mi parte / total pagado

Notas (texto largo; indicador visual si no vacío)
