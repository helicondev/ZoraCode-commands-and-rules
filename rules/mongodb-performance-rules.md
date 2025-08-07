# MongoDB Performance Rules

Reglas de optimización de performance para MongoDB.

## Connection Management
1. **Connection pooling**: configurar pool size basado en carga
2. **Connection reuse**: reutilizar conexiones, no crear por operación
3. **Timeout settings**: configurar timeouts apropiados por entorno
4. **Monitor connections**: alertas por agotamiento de pool

## Memory Management
1. **Working set**: mantener working set en RAM
2. **Index size**: índices deben caber en memoria
3. **Document size**: documentos grandes afectan performance
4. **Memory monitoring**: alertas por uso excesivo de memoria

## Sharding Strategy
1. **Shard key selection**: clave que distribuya uniformemente
2. **Avoid hotspots**: evitar claves monotónicamente crecientes
3. **Query routing**: queries deben incluir shard key cuando posible
4. **Chunk balancing**: monitorear distribución de chunks

## Monitoring Requirements
1. **Slow query log**: habilitar para queries >100ms
2. **Profiler**: usar en desarrollo, nivel 1 en producción
3. **Metrics collection**: WiredTiger, operations, connections
4. **Alerting thresholds**: definir umbrales por métrica crítica