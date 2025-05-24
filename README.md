# Proyecto de Control de Péndulo Invertido

Este repositorio contiene el desarrollo completo de un sistema de control para un péndulo invertido implementado con un ESP32.

## Práctica 4: Implementación del Controlador PID

### Objetivo

Desarrollar una biblioteca de control PID personalizada en C++ para el ESP32, con tres variantes de control PID, y probar su funcionamiento previo a la integración con el péndulo invertido real.

### Descripción

Se han implementado tres versiones de un controlador PID:

1. **PID básico** (Implementación de un controlador PID en tiempo discreto basado en la fórmula directa con términos proporcional, integral y derivativo).
2. **PID como filtro IIR** (Controlador PID que calcula la salida usando una fórmula similar a un filtro digital.).
3. **PID con derivada filtrada** (Incluye un filtro pasabajo para reducir el ruido del término derivativo).

Cada implementación fue encapsulada en una clase separada dentro de una biblioteca propia llamada "PIDController".

### Estructura del Proyecto
PIDController/

├── src/

│     ├── PIDBasico.h

│     ├── PIDBasico.cpp

│     ├── PIDFiltroIIR.h

│     ├── PIDFiltroIIR.cpp

│     ├── PIDDerivadaFiltrada.h

│     └── PIDDerivadaFiltrada.cpp

├── examples/

│     ├── PIDBasico_Example/

│     │     └── PIDBasico_Example.ino

│     ├── PIDFiltroIIR_Example/

│     │     └── PIDFiltroIIR_Example.ino

│     └── PIDDerivadaFiltrada_Example/

│     │    └── PIDDerivadaFiltrada_Examplee.ino

├── keywords.txt

└── library.properties
