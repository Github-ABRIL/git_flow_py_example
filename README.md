# Git Flow Py Example

Este repositorio demuestra un ejemplo de flujo de trabajo utilizando Git Flow. A continuación, se describen los pasos y procesos usados en este ejemplo.

## Configuración Inicial

Se creó un nuevo directorio y se inicializó un repositorio de Git. Se agregó un remoto llamado `origin` apuntando al repositorio de GitHub. Se añadió el primer archivo `main.py` y se hizo push a la rama `main` del repositorio remoto.

## Desarrollo Continuo

Se estableció una rama `develop` como rama central para el desarrollo. Todos los desarrollos continuos y las integraciones de características se hacen en esta rama.

## Características Nuevas

Para cada nueva característica, se creó una rama específica desde `develop`. Esto aísla el desarrollo de nuevas características hasta que estén listas para ser integradas al flujo principal de desarrollo.

### Finalización de Características

Una vez que las características estaban completas, se fusionaron de vuelta a la rama `develop`. Esto se hizo con la opción `--no-ff` para mantener la historia de la rama de característica.

## Preparación de Release

Con las características listas para ser lanzadas, se creó una rama `release` desde `develop`. Esta rama se usó para preparaciones finales de la release, como la actualización de metadatos y pruebas finales.

## Lanzamiento de la Release

Después de la preparación final, la rama `release` se fusionó a `main` y se etiquetó con un número de versión. Esto marcó un punto fijo en la historia del proyecto representando una versión de producción.

## Hotfixes

Si se detectaban errores en `main`, se creaban ramas `hotfix` para realizar correcciones rápidas y directas. Una vez arreglados, los hotfixes se fusionaron tanto a `main` como a `develop` para mantener la coherencia en el código y las correcciones.

## Colaboración

Se empujaron todas las ramas pertinentes al repositorio remoto para mantener la colaboración y el seguimiento centralizado del progreso del proyecto.

---

Para más detalles sobre cómo usar y entender este flujo de trabajo, consulta la historia del repositorio y las ramas en GitHub.
