# Reglas de Organización de Archivos

Este proyecto tiene reglas estrictas sobre donde ubicar cada tipo de archivo.

## Separación Obligatoria de Archivos
1. **UN ARCHIVO = UNA RESPONSABILIDAD** - Nunca mezcles tipos diferentes
2. **INTERFACES** van en archivos separados terminados en .interface.ts
3. **ENUMS** van en archivos separados terminados en .enum.ts
4. **DTOs** van en archivos separados terminados en .dto.ts
5. **TYPES** van en archivos separados terminados in .type.ts
6. **CONSTANTS** van en archivos separados terminados en .constant.ts

## Ubicaciones por Tipo de Archivo
1. **Interfaces de Dominio**: `/src/domain/interfaces/`
2. **Value Objects**: `/src/domain/value-objects/`
3. **Entidades**: `/src/domain/entities/`
4. **DTOs de Request/Response**: `/src/presentation/dtos/`
5. **DTOs de Aplicación**: `/src/application/dtos/`
6. **Enums de Dominio**: `/src/domain/enums/`
7. **Tipos Compartidos**: `/src/shared/types/`
8. **Constantes de Configuración**: `/src/config/constants/`

## Prohibiciones Absolutas
1. **NUNCA** coloques interfaces dentro de archivos de clases
2. **NUNCA** definas enums dentro de servicios o controladores
3. **NUNCA** mezcles DTOs con lógica de negocio
4. **NUNCA** pongas types compartidos dentro de módulos específicos
5. **NUNCA** definas constantes inline cuando pueden ser reutilizadas