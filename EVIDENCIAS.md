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
