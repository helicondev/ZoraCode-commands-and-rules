# Environment Management Rules

Gestión de configuraciones y environments.

## Configuration Management
1. **Environment variables**: toda configuración via env vars
2. **Secrets management**: nunca hardcodear secrets en código
3. **Explicit configuration**: NO valores por defecto, todas las variables deben ser explícitas
4. **Validation**: validación estricta de configuración al startup, fallar si falta alguna variable crítica

## Environment Separation
1. **Development isolation**: datos de dev aislados de producción
2. **Staging parity**: staging debe ser idéntico a producción en configuración
3. **Feature flags**: usar para deployment gradual de features
4. **Blue-green deployment**: estrategia de deployment sin downtime

## Configuration Validation
1. **Required variables**: aplicación debe fallar al inicio si faltan variables críticas
2. **Type validation**: validar tipos de datos de variables (number, boolean, url)
3. **Environment-specific validation**: diferentes validaciones por ambiente
4. **Configuration documentation**: documentar todas las variables requeridas por ambiente

## Monitoring Per Environment
1. **Environment tagging**: tags claros en logs y métricas
2. **Different thresholds**: umbrales diferentes por ambiente
3. **Access control**: permisos restrictivos por ambiente
4. **Data retention**: políticas diferentes por criticidad del ambiente