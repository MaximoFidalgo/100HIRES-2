# Mi entorno de desarrollo

Este documento resume los pasos que seguí para preparar **Cursor**, **Git**, **GitHub** y las extensiones de **Claude** y **Codex**.

## 1. Instalar Cursor

- Descargué [Cursor](https://cursor.com) desde la página oficial.
- Instalé el editor y lo configuré como entorno principal para programar con asistencia de IA.

## 2. Extensiones: Claude y Codex

- Desde el marketplace de extensiones de Cursor (similar a VS Code), instalé:
  - **Claude** (extensión de Anthropic).
  - **Codex** (extensión relacionada con flujos de trabajo asistidos por IA).
- Estas extensiones permiten usar los modelos y herramientas correspondientes dentro del editor.

## 3. Cuenta de GitHub

- Creé una cuenta en [GitHub](https://github.com).
- GitHub sirve para guardar el código en la nube, colaborar y usar control de versiones con `git`.

## 4. Vincular Claude y Codex con Cursor

- Configuré las cuentas o API keys necesarias en la configuración de Cursor o de cada extensión, según lo que pidiera el asistente al iniciar sesión o al usar la función por primera vez.
- Así Cursor puede autenticarse y usar Claude y Codex sin salir del editor.

## 5. Instalar Git

- Descargué e instalé [Git](https://git-scm.com) en mi equipo (Windows).
- Git es la herramienta de línea de comandos que se conecta con GitHub para clonar, hacer commit y subir cambios.

## 6. Crear un repositorio en GitHub

- En la web de GitHub, creé un **nuevo repositorio** (vacío o con la opción de incluir un README, según el caso).
- Anoté la URL del repositorio (por ejemplo `https://github.com/usuario/nombre-repo.git`) para enlazarlo con la carpeta local.

## 7. Subir este `README.md` a GitHub

- En la carpeta del proyecto en mi PC, inicialicé o cloné el repo y añadí este archivo `README.md`.
- Usé los comandos habituales de Git, por ejemplo:

  ```bash
  git add README.md
  git commit -m "Añadir README con los pasos de configuración"
  git push origin main
  ```

  *(La rama puede llamarse `main` o `master` según cómo esté creado el repositorio en GitHub.)*

## Resumen

| Paso | Qué hice |
|------|----------|
| Editor | Instalé Cursor |
| IA en el editor | Instalé extensiones Claude y Codex y las vinculé a Cursor |
| Nube y cuenta | Creé cuenta y repositorio en GitHub |
| Control de versiones | Instalé Git y subí este README al repositorio |

---

Si más adelante añades proyectos de código en esta misma carpeta, puedes ampliar este README con instrucciones de instalación y uso del proyecto.
