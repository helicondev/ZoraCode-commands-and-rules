# Principios SOLID

Este proyecto adhiere estrictamente a los principios SOLID.

## Single Responsibility Principle (SRP)
1. Cada clase debe tener una sola razón para cambiar
2. Los servicios deben tener una responsabilidad específica y bien definida
3. Separa concerns: validación, transformación, persistencia
4. Un método debe hacer una sola cosa conceptualmente

## Open/Closed Principle (OCP)
1. Usa interfaces y abstracciones para extensibilidad
2. Implementa Strategy pattern para algoritmos variables
3. Evita modificar código existente, extiende funcionalidad
4. Usa decorators para añadir comportamiento

## Liskov Substitution Principle (LSP)
1. Las implementaciones deben ser intercambiables con sus interfaces
2. No cambies el comportamiento esperado en las implementaciones
3. Respeta los contratos definidos por las interfaces
4. Las precondiciones no pueden ser más restrictivas

## Interface Segregation Principle (ISP)
1. Crea interfaces específicas y cohesivas
2. Los clientes no deben depender de métodos que no usan
3. Prefiere múltiples interfaces pequeñas sobre una grande
4. Usa composition sobre inheritance

## Dependency Inversion Principle (DIP)
1. Depende de abstracciones, no de concreciones
2. Los módulos de alto nivel no deben depender de módulos de bajo nivel
3. Usa inyección de dependencias para inversión de control
4. Define interfaces en las capas que las consumen