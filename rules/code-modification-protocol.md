# Protocolo para Modificar Código Existente

Antes de modificar cualquier código existente, DEBES seguir este protocolo estricto.

## Análisis Obligatorio Pre-Modificación
1. **LEE COMPLETAMENTE** el archivo que vas a modificar
2. **ENTIENDE** el propósito y responsabilidad actual del código
3. **IDENTIFICA** todos los lugares donde se usa la funcionalidad
4. **VERIFICA** si la modificación afecta otros archivos o módulos
5. **CONFIRMA** que entiendes las implicaciones de los cambios

## Reglas de Modificación Mínima
1. **NUNCA** refactorices código que funciona a menos que sea específicamente solicitado
2. **MODIFICA** solo lo mínimo necesario para resolver el problema
3. **PRESERVA** la estructura y patrones existentes del archivo
4. **MANTÉN** la consistencia con el estilo de código existente
5. **NO CAMBIES** nombres de variables/funciones existentes sin justificación

## Validación de Impacto
1. **ANTES** de modificar, lista todos los archivos que podrían verse afectados
2. **VERIFICA** que los cambios no rompen contratos existentes
3. **CONFIRMA** que las interfaces públicas permanecen compatibles
4. **VALIDA** que no introduces breaking changes sin justificación
5. **ASEGÚRATE** de que los tests existentes siguen pasando conceptualmente

## Documentación de Cambios
1. **EXPLICA** por qué cada cambio es necesario
2. **JUSTIFICA** cualquier modificación de código existente funcional
3. **DOCUMENTA** cualquier cambio de comportamiento
4. **INDICA** si se requieren cambios en otros archivos