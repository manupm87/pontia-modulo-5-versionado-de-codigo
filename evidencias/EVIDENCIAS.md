# Opciones de protección de la rama principal(main)
(target default branch -main-)
- Restrict deletions
- Require a pull request before merging
- Require approvals: 1
    - Dismiss stale pull request approvals when new commits are pushed
    - Require review from Code Owners
    - Require conversation resolution before merging
    - Block force pushes

# Por qué es recomendable proteger la rama principal(main)
- Evita que se realicen cambios no deseados en la rama principal
- Asegura que los cambios en la rama principal sean revisados y aprobados por al menos una persona
- Mantiene la rama principal estable y libre de errores
- Facilita la colaboración en equipo
- Permite mantener un historial de cambios limpio y ordenado

# Configuración de .gitignore
*.log # Ignora todos los archivos que terminan en .log en cualquier lugar del repositorio
__pycache__/ # Ignora el directorio __pycache__ y todo su contenido

# Enlace al repositorio
https://github.com/manupm87/pontia-modulo-5-versionado-de-codigo

# Explicación del flujo de trabajo
Para cada ejercicio propuesto:
1. Leer el ejercicio propuesto
2. Crear una sección en un archivo word para ir pegando evidencias en formato imagen
3. Realizar los cambios en el repositorio local y remoto
4. Tomar capturas de pantalla de los cambios
5. Pegar las capturas en el archivo word

# Descripción de cómo se produjo y resolvió el conflicto
Dos ramas continenen cambios en el mismo archivo, en la misma linea. Puesto que una rama se "mergea" a main antes que la otra, cuando la segunda
se intenta mergear a main, se produce un conflicto.

En este caso ambos cambios eran correctos, así que se eligió la opción de mantener ambos cambios.

# Brebe explicación del workflow de GitHub Actions
Se ha creado un workflow que sólo se ejecuta de manera manual (sobre cualquier rama). Este workflow solicita dos parámetros, nombre y apellidos. Los combina y los imprime por la consola.

El workflow se ejecuta en un container "ubuntu-latest".
