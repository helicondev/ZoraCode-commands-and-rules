# Reglas de Imports y Dependencias

Este proyecto tiene reglas estrictas sobre como importar y organizar dependencias.

## Orden de Imports Obligatorio
1. **Librerías externas** (node_modules) primero
2. **Imports internos del framework** (NestJS)
3. **Imports de capas arquitectónicas** en orden: domain → application → infrastructure → presentation
4. **Imports relativos** del mismo módulo al final
5. **Separar grupos** con líneas en blanco

## Reglas de Dependencias Entre Capas
1. **Domain** NO puede importar de ninguna otra capa
2. **Application** puede importar solo de Domain
3. **Infrastructure** puede importar de Domain y Application
4. **Presentation** puede importar de Domain, Application e Infrastructure (solo para inyección)

## Imports Barrel Prohibidos
1. **NUNCA** uses imports de barrel (index.ts) que exporten todo
2. **SIEMPRE** importa específicamente lo que necesitas
3. **EVITA** re-exports innecesarios que acoplen módulos
4. **USA** imports directos para mejor tree-shaking

## Path Mapping Obligatorio
1. **USA** path absolutos configurados en tsconfig para imports internos
2. **EVITA** imports relativos profundos (../../..)
3. **CONFIGURA** aliases para cada capa arquitectónica
4. **MANTÉN** consistencia en todos los imports del proyecto

## Validación de Imports
1. Antes de crear un import, verifica que no viola reglas de capas
2. No importes implementaciones concretas en capas superiores
3. Usa interfaces para desacoplar dependencias
4. Verifica que el import no crea dependencias circulares