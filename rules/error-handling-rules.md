# Error Handling Rules

Manejo consistente de errores en toda la aplicación.

## Exception Hierarchy
1. **Custom exceptions**: jerarquía clara de excepciones de dominio
2. **Error codes**: códigos únicos para cada tipo de error
3. **Error categories**: business, validation, infrastructure, external
4. **Propagation rules**: cuándo capturar vs. propagar errores

## Logging Standards
1. **Error context**: incluir contexto suficiente para debugging
2. **Correlation IDs**: trackear errores a través de requests
3. **Log levels**: usar niveles apropiados por severidad
4. **Sensitive data**: nunca loggear información sensible

## User Communication
1. **User-friendly messages**: mensajes comprensibles para usuarios
2. **Internationalization**: mensajes traducibles
3. **Error recovery**: sugerir acciones de recuperación cuando posible
4. **Support information**: incluir referencias para soporte técnico

## Monitoring & Alerting
1. **Error rates**: alertas por incremento en tasa de errores
2. **Critical path errors**: alertas inmediatas para flujos críticos
3. **Error trending**: análisis de tendencias de errores
4. **Recovery metrics**: tiempo promedio de recuperación