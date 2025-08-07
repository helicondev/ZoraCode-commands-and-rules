# Ubicación por Capa Arquitectónica

Cada archivo debe ubicarse en la capa arquitectónica correcta según su responsabilidad.

## Domain Layer (/src/domain/)

1. Entities: Objetos de negocio con identidad única
2. DTOs: Objetos de transferencia de datos del dominio organizados por contexto
3. Enums: Enumeraciones que representan conceptos de dominio
4. Repository Interfaces: Contratos de persistencia definidos por el dominio
5. Schemas: Esquemas de base de datos (específico para MongoDB/Mongoose)
6. Domain Interfaces: Contratos de servicios externos (cache, stores)

## Application Layer (/src/application/)

1. Use Cases: Casos de uso específicos organizados por contexto de negocio
2. Application Services: Servicios que orquestan múltiples casos de uso
3. Command/Query Handlers: Manejadores CQRS si se implementa
4. Application Events: Eventos de aplicación
5. Application Interfaces: Puertos definidos por la aplicación

## Infrastructure Layer (/src/infrastructure/)

1. Repositories: Implementaciones concretas de persistencia
2. Controllers: Controladores HTTP/REST
3. Modules: Módulos de configuración e inyección de dependencias
4. Services: Servicios de infraestructura (Redis, externos)
5. Factories: Patrones factory para creación de objetos complejos
6. Adapters: Implementaciones de interfaces de dominio/aplicación

## Common Layer (/src/common/)

1. Decorators: Decoradores reutilizables transversales
2. Services: Servicios compartidos entre capas
3. Utils: Utilidades y helpers compartidos
4. Guards: Guards de seguridad y autorización
5. Interceptors: Interceptores transversales

## Configuration Layer (/src/config/)

1. Configuration: Archivos de configuración centralizada
2. Environment: Validadores y configuración de entorno
3. Logger: Configuración de logging
4. Database: Configuración de conexiones a bases de datos