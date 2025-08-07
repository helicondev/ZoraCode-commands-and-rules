# Manejo de Errores

Este proyecto tiene políticas específicas para manejo de errores.

## Excepciones de Dominio
1. Crea excepciones específicas por tipo de error de negocio
2. Las excepciones de dominio extienden de una clase base común
3. Incluye contexto relevante en el mensaje de error
4. No expongas detalles técnicos en excepciones de dominio

## Propagación de Errores
1. No captures excepciones que no puedes manejar apropiadamente
2. Re-throw excepciones después de logear con contexto
3. Transforma excepciones técnicas en errores de dominio en boundaries
4. Usa Result types o Either monads para operaciones que pueden fallar

## Logging de Errores
1. Logea errores con nivel apropiado (error, warn, info)
2. Incluye stack traces solo para errores inesperados
3. Añade contexto de negocio relevante (userId, transactionId)
4. No logees información sensible (passwords, tokens)

## Códigos de Estado HTTP
1. Mapea excepciones de dominio consistentemente a HTTP status
2. Usa 400 para errores de validación
3. Usa 404 para recursos no encontrados
4. Usa 409 para conflictos de reglas de negocio
5. Reserva 500 para errores técnicos no manejados