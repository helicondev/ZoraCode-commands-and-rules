# Code Organization Rules

Estructura y organización del código fuente.

## File Structure
1. **File naming**: kebab-case para archivos, PascalCase para clases
2. **Directory depth**: máximo 5 niveles de profundidad
3. **File size**: máximo 300 líneas por archivo
4. **Single responsibility**: un concepto principal por archivo

## Import/Export Management
1. **Barrel exports**: usar index.ts para exportaciones de módulos
2. **Import order**: third-party, internal, relative imports
3. **Circular dependencies**: detección automática y prohibición
4. **Unused imports**: limpieza automática en pre-commit hooks

## Documentation Requirements
1. **README per module**: documentación clara por módulo
2. **API documentation**: OpenAPI/Swagger para todos los endpoints
3. **Code comments**: solo para lógica compleja o no obvia
4. **Architecture decisions**: ADRs para decisiones importantes

## Version Control
1. **Commit messages**: formato conventional commits obligatorio
2. **Branch naming**: feature/, bugfix/, hotfix/ prefixes
3. **PR requirements**: review obligatorio, tests passing, no conflicts
4. **Release management**: semantic versioning estricto