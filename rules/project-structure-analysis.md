# Análisis de Estructura de Proyecto

Antes de crear cualquier archivo o código, DEBES analizar completamente la estructura existente del proyecto.

## Proceso Obligatorio Previo
1. **SIEMPRE** examina la estructura de directorios completa antes de crear código
2. **IDENTIFICA** patrones existentes de organización de archivos
3. **LOCALIZA** donde están ubicados archivos similares al que vas a crear
4. **VERIFICA** convenciones de nomenclatura ya establecidas en el proyecto
5. **CONFIRMA** la capa arquitectónica apropiada para el nuevo código

## Análisis de Contexto Requerido
1. Revisa archivos existentes del mismo tipo (DTOs, interfaces, enums, servicios)
2. Identifica el módulo o bounded context al que pertenece la nueva funcionalidad
3. Examina imports existentes para entender dependencias entre capas
4. Verifica si ya existe funcionalidad similar que puedas reutilizar
5. Confirma que no estás duplicando código existente

## Verificación de Ubicación
1. **NUNCA** asumas la ubicación de un archivo sin revisar la estructura
2. **SIEMPRE** coloca archivos en el directorio que corresponde a su tipo y responsabilidad
3. **CONFIRMA** que la ubicación sigue las convenciones arquitectónicas del proyecto
4. **VALIDA** que no estás violando la separación de capas