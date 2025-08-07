# Gestión de Dependencias

Este proyecto tiene políticas específicas sobre librerías y dependencias.

## Librerías Prohibidas
1. **NO usar @nestjs/mongoose** - Usar mongoose nativo directamente
2. **NO usar nest-winston** - Usar winston nativo directamente
3. **NO usar librerías que wrappean** funcionalidad básica innecesariamente
4. Evita dependencias que acoplan el dominio a frameworks específicos

## Políticas de Mongoose
1. Usar mongoose directamente sin abstracciones de NestJS
2. Los esquemas de Mongoose van en la capa de infraestructura
3. Implementa el patrón Repository manualmente
4. No uses decoradores de mongoose en entidades de dominio
5. Separa modelos de mongoose de entidades de dominio

## Políticas de Winston
1. Usar winston directamente sin wrappers de NestJS
2. Configura winston en la capa de infraestructura
3. Crea interfaces de logging en el dominio
4. Usa dependency injection para proveer logger configurado
5. No importes winston directamente en servicios de dominio

## Evaluación de Nuevas Dependencias
1. Justifica cada nueva dependencia con casos de uso específicos
2. Prefiere librerías con APIs simples y sin magic
3. Evalúa el tamaño del bundle y tree-shaking support
4. Verifica que la librería no viole principios arquitectónicos