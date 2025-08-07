# Consistencia de Nomenclatura en el Proyecto

DEBES mantener consistencia con los nombres existentes en todo el proyecto.

## Análisis de Patrones Existentes
1. **BUSCA** patrones de nomenclatura similares en el codebase existente
2. **IDENTIFICA** convenciones específicas del dominio de negocio
3. **VERIFICA** como se nombran entidades similares en otros módulos
4. **CONFIRMA** terminología de negocio ya establecida
5. **REUTILIZA** nombres existentes cuando sea apropiado

## Reglas de Consistencia Terminológica
1. **SI** existe una entidad "User", NO crees "Person" o "Account" para lo mismo
2. **SI** existe un patrón "CreateXxxDto", MANTÉN ese patrón para todos los DTOs
3. **SI** existe un sufijo específico como "Repository", ÚSALO consistentemente
4. **NO CAMBIES** terminología de negocio ya establecida sin justificación
5. **REUTILIZA** Value Objects existentes antes de crear nuevos similares

## Verificación de Unicidad
1. **ANTES** de crear una nueva clase, verifica que no existe una similar
2. **ANTES** de crear un nuevo enum, busca si ya existe uno equivalente
3. **ANTES** de crear un DTO, confirma que no hay uno reutilizable
4. **ANTES** de definir constantes, busca si ya están definidas
5. **EVITA** duplicar conceptos con nombres diferentes

## Abstracción de Nombres
1. **USA** nombres específicos del dominio, no términos técnicos genéricos
2. **PREFIERE** "OrderStatus" sobre "Status" cuando sea específico de órdenes
3. **EVITA** nombres ambiguos que podrían aplicar a múltiples conceptos
4. **SÉ** específico: "UserRegistrationDto" no "CreateDto"