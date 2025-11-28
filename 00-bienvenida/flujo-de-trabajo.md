# 🛠️ Flujo de Trabajo y Guía de Contribución

Esta guía establece los protocolos técnicos para aportar material al repositorio **LINUDECX Base de Conocimiento**. Seguir estos pasos garantiza que la información se mantenga ordenada y accesible para todos.

Sobre la mforma de trabaar en el semillero, deberes y derechos como miembro, revisa el archivo **[Metodologia Semillero](./METODOLOGIA-SEMILLERO.md)**

---

## 1. Estrategia de Ramas (Git Flow)

Para mantener la integridad del historial, la rama `main` está **protegida**. Nadie puede hacer cambios directos sobre ella.

### Pasos para colaborar:

1.  **Actualiza tu repositorio local:** Antes de empezar, asegúrate de tener la última versión.
    ```bash
    git checkout main
    git pull origin main
    ```
2.  **Crea una nueva rama:** Nunca trabajes en `main`. Nombra tu rama según lo que vas a hacer:
    * Para un proyecto nuevo: `proyecto/nombre-del-proyecto`
    * Para una corrección: `fix/nombre-del-error`
    * Para una guía nueva: `docs/nombre-guia`

    ```bash
    # Ejemplo
    git checkout -b proyecto/sistema-riego-iot
    ```
3.  **Realiza tus cambios y commits.**
4.  **Sube tu rama:**
    ```bash
    git push origin proyecto/sistema-riego-iot
    ```
5.  **Crea un Pull Request (PR):** Ve a GitHub y abre una solicitud para fusionar tu rama con `main`.
    * **Revisores:** Tu PR debe ser aprobado por el Líder del Semillero o la Directora antes de ser mezclado.

---

## 2. Nomenclatura (Naming Convention)

Para garantizar compatibilidad y orden, usamos estrictamente **snake_case**.

* **Carpetas y Archivos:** Todo en minúsculas, separado por guiones medios (`-`) o bajos (`_`).
    * ✅ `manual-tecnico.pdf`
    * ✅ `diagrama_clases.png`
    * ❌ `Manual Tecnico.pdf` (Evitar espacios)
    * ❌ `DiagramaClases.png` (Evitar CamelCase)

* **Archivos Especiales:** Solo los archivos estándar de documentación van en MAYÚSCULAS:
    * `README.md`
    * `BITACORA.md`
    * `LINKS.md`
    * `LICENSE`

---

## 3. Protocolo de Commits (Conventional Commits)

Usamos una estructura estandarizada para los mensajes de confirmación. Esto nos permite leer el historial rápidamente.

**Estructura:** `<tipo>: <descripción breve en español>`

| Tipo | Uso | Ejemplo |
| :--- | :--- | :--- |
| **feat** | Contenido nuevo importante (Proyectos, Guías) | `feat: agregar documentacion inicial proyecto arandanos` |
| **fix** | Corrección de errores (Enlaces rotos, typos) | `fix: corregir enlace roto en directorio alumni` |
| **docs** | Cambios menores en documentación o formato | `docs: mejorar redacción en guia de git` |
| **style**| Cambios de estilo visual (Markdown, espacios) | `style: ajustar formato de tablas en readme` |
| **chore**| Tareas de mantenimiento (Mover archivos, licencias) | `chore: reorganizar carpetas del año 2024` |

---

## 4. Checklist para Nuevos Proyectos

Si vas a subir un Proyecto de Grado o Investigación terminado, tu carpeta en `02-proyectos/AÑO/nombre-proyecto` debe contener obligatoriamente como MÍNIMO:

- [ ] **Carpeta copiada de la plantilla:** Usa `02-proyectos/plantilla-proyecto` como base.
- [ ] **README.md:** Completo con título, autores, resumen y estado del proyecto.
- [ ] **BITACORA.md:** Con la historia, decisiones, dificultades y lecciones aprendidas (post-mortem).
- [ ] **LINKS.md:** Con los enlaces al código fuente (repositorios de desarrollo o del proyecto en general), videos en YouTube, simulaciones y demás contenido relacionado.
- [ ] **Diagramas:** Al menos un diagrama de arquitectura o diseño en la carpeta `entregables/diagramas`.
- [ ] **Multimedia:** Fotos del prototipo o actividad en `multimedia/fotos` (Recuerda: **No videos pesados, solo enlaces**).

---

## 5. Manejo de Multimedia

* **Imágenes:** Formatos `.png`, `.jpg`, `.svg`. Intenta que no pesen más de **2MB**.
* **Videos:** **Prohibido subir archivos de video (.mp4, .mov)** directamente al repositorio. Súbelos a YouTube (como "Público" o "No listado") y coloca el enlace en el archivo `VIDEOS.md` o `LINKS.md`.

---
*Siguiendo estas reglas, construimos un legado duradero para LINUDECX y la sociedad.*