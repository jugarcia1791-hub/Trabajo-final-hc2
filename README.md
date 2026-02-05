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
-----------------------------------------
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
 
 ------
 npx @tailwindcss/cli -i ./src/input.css -o ./src/output.css --watch
 # Agregar remoto (después de crear el repo en GitHub)
git remote add origin URL_DEL_REPO
 
 https://github.com/jugarcia1791-hub/TRABAJO-FINAL-HC1.git

git init (iniciar)

# Ver todas las ramas locales
git branch
# Renombrar rama master a main localmente
git branch -m master main