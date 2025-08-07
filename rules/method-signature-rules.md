# Method Signature Rules

Reglas obligatorias para definición de métodos y sus signatures.

## Parameter Management
1. **Máximo 3 parámetros primitivos**: si necesitas más de 3 parámetros, usar interfaz
2. **Parámetros relacionados**: agrupar parámetros que conceptualmente van juntos en una interfaz
3. **Parámetros opcionales**: usar interfaces para manejar parámetros opcionales de manera clara
4. **Orden de parámetros**: parámetros obligatorios primero, opcionales después

## Return Type Definition
1. **Tipos primitivos únicos**: está permitido retornar string, number, boolean directamente
2. **Múltiples valores**: cualquier retorno con más de un campo debe usar interfaz
3. **Tipos union complejos**: evitar union types complejos, usar interfaces discriminated
4. **Return type explícito**: siempre declarar el tipo de retorno, nunca usar inferencia implícita

## Interface Requirements
1. **Naming convention**: sufijo apropiado según contexto (Params, Result, Response, Options)
2. **Single purpose**: cada interfaz debe tener una responsabilidad específica
3. **Immutable by default**: preferir readonly properties cuando sea apropiado
4. **Optional vs Required**: ser explícito sobre qué campos son opcionales

## Method Documentation
1. **JSDoc obligatorio**: para métodos públicos que reciben interfaces
2. **Parameter description**: describir cada parámetro de la interfaz
3. **Return description**: explicar qué representa cada campo del objeto retornado
4. **Business context**: explicar el propósito del método en contexto de negocio

## Validation Rules
1. **Input validation**: validar parámetros de entrada usando class-validator cuando aplique
2. **Type safety**: garantizar type safety tanto en entrada como en salida
3. **Null safety**: manejar casos de null/undefined explícitamente
4. **Error handling**: definir qué excepciones puede lanzar el método

## Consistency Standards
1. **Naming patterns**: usar patrones consistentes para nombres de interfaces (CreateUserParams, UserResult)
2. **Field naming**: mantener nomenclatura consistente entre interfaces relacionadas
3. **Data transformation**: ser explícito sobre transformaciones entre tipos de entrada y salida
4. **Versioning**: considerar versionado de interfaces para cambios breaking