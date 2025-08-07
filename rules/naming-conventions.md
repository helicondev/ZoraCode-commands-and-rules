# Convenciones de Nomenclatura

Este proyecto sigue convenciones estrictas de nomenclatura.

## Variables y Funciones
1. Usa camelCase para variables, funciones y métodos
2. Los nombres deben ser descriptivos y auto-documentados
3. Evita abreviaciones ambiguas (usa userRepository no userRepo)
4. Los booleans deben comenzar con is, has, can, should

## Clases e Interfaces
1. Usa PascalCase para clases, interfaces y tipos
2. Las interfaces no deben tener prefijo I
3. Los tipos de dominio no deben tener sufijos técnicos
4. Las implementaciones pueden tener sufijos descriptivos (UserMongoRepository)

## Archivos y Directorios
1. Usa kebab-case para nombres de archivos
2. Los directorios siguen la estructura arquitectónica
3. Un archivo por clase/interface pública
4. Los archivos de test terminan en .spec.ts o .test.ts

## Constantes y Enums
1. Usa SCREAMING_SNAKE_CASE para constantes
2. Los enums usan PascalCase para el nombre y claves
3. Agrupa constantes relacionadas en objetos o namespaces
4. Prefiere const assertions sobre enums cuando sea apropiado