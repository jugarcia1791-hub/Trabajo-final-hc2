# Trabajo-final-hc2

Se debe presentar avances de el proyecto final de HTML

# Enero 22 del 2026

Apuntes de HTML Y CSS

-Creacion del Repositorio

-Vinculacion con Editor de Codigo
Opcion Source Control>Clone repository

-Configurar Identidad de github
se despliega terminal
git config --global user.email "tu-email@example.com"
git config --global user.name "Tu Nombre"

---

Despues de vincular, se empiezan lo cambios locales o creacion de documentos
en la terminal
git status
git add .
git commit -m "Descripción del cambio"
git push origin main

# Enero 23 del 2026

-Integracion con Tailwindcss
npm install tailwindcss @tailwindcss/cli

src/input.css
@import "tailwindcss";

---
npx @tailwindcss/cli -i ./css/input.css -o ./css/output.css --watch
 (compilar css )

# Agregar remoto (después de crear el repo en GitHub)

git remote add origin URL_DEL_REPO

git init (iniciar)

# Ver todas las ramas locales

git branch

# Renombrar rama master a main localmente

git branch -m master main

# 05 /02/26

comandos bash
Listar todos los archivos en una carpeta:
ls
mirar ubicacion actual:
pwd
ir a carpeta seleccionada:
cd archivo destino

# 06/02/26

creacion del index
-header
-barra de navegacion
-body

#comando para instalar tailwind
-Integracion con Tailwindcss
npm install tailwindcss @tailwindcss/cli

src/input.css
@import "tailwindcss";
npx @tailwindcss/cli -i ./src/input.css -o ./src/output.css --watch (compilacion en vivo)
npx serve . (server en vivo)

#07/02/26

<!-- En cada página, cambia manualmente la clase "active" -->
<nav>
    <a href="index.html" class="{{ 'active' if page == 'home' }}">Inicio</a>
    <a href="blog.html" class="{{ 'active' if page == 'blog' }}">Blog</a>
</nav>
# 18/02/26
se agregan cambios a la estreuctura de el proyecto, se agregan imagenes para la pagina principal y su contenido

21/02/26
stilo

<style>
      .campo-obligatorio {
        margin: 15px 0;
        position: relative;
      }

      label {
        cursor: pointer;
        display: inline-block;
        padding-left: 30px;
        position: relative;
      }

      label:before {
        content: "";
        position: absolute;
        left: 0;
        top: 1px;
        width: 20px;
        height: 20px;
        border: 2px solid #ccc;
        border-radius: 4px;
        background: white;
      }

      input[type="checkbox"] {
        opacity: 0;
        position: absolute;
      }

      input[type="checkbox"]:checked + label:before {
        background: #4caf50;
        border-color: #4caf50;
      }

      input[type="checkbox"]:checked + label:after {
        content: "";
        position: absolute;
        left: 6px;
        top: 6px;
        width: 8px;
        height: 8px;
        border: solid white;
        border-width: 0 2px 2px 0;
        transform: rotate(45deg);
      }

      .error-message {
        color: #d32f2f;
        font-size: 0.85em;
        margin-top: 5px;
      }
    </style>