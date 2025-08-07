# MongoDB Design Rules

Reglas obligatorias para diseño y uso de MongoDB.

## Schema Design
1. **Embedding vs Referencing**: embedder documentos que se consultan juntos frecuentemente
2. **Máximo 16MB por documento**: mantener documentos dentro del límite
3. **Arrays no deben crecer sin límite**: usar paginación o referencias para arrays grandes
4. **Desnormalización estratégica**: duplicar datos para optimizar queries frecuentes

## Naming Conventions
1. **Colecciones**: plural, camelCase
2. **Campos**: camelCase consistente
3. **IDs**: usar ObjectId por defecto, custom IDs solo cuando necesario
4. **Campos booleanos**: prefijo "is", "has", "can"

## Indexing Strategy
1. **Compound indexes**: orden de campos por selectividad (más selectivo primero)
2. **Query patterns**: crear índices basados en patterns reales de consulta
3. **Background creation**: todos los índices en producción se crean en background
4. **Index monitoring**: revisar índices no utilizados mensualmente

## Query Optimization
1. **Projection**: siempre especificar campos necesarios
2. **Limit y skip**: usar limit en todas las queries, evitar skip grandes
3. **Aggregation pipeline**: preferir sobre queries complejas con código
4. **Explain plans**: revisar explain() para todas las queries críticas

## Data Consistency
1. **Transactions**: usar solo cuando ACID es crítico
2. **Write concerns**: acknowledged para writes importantes
3. **Read concerns**: majority para datos críticos
4. **Eventual consistency**: aceptar para datos no críticos