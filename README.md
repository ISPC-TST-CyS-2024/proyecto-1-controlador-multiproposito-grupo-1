[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/T1dZM0_Y)

# Proyecto #1 Controlador Multipropósito

## ControladorMx

**El objetivo principal del proyecto es desarrollar un controlador universal llamado "ControladorMx" que permita recibir diferentes tipos de entradas, generar diferentes tipos de salidas y proporcionar una interfaz de visualización y ajuste mediante un display local.**  

### **Objetivos del Proyecto:**

1. Implementar un sistema versátil de entradas de control:  
   - El controlador debe ser capaz de aceptar sensores resistivos, entradas analógicas y digitales, y permitir la temporización para la entrada digital.
    
2. Desarrollar un sistema de salidas de control flexible:  
   - El controlador debe generar salidas PWM, salidas analógicas y digitales, permitiendo que cada salida defina una función lógica basada en las entradas digitales.
     
3. Crear una interfaz de usuario intuitiva y accesible:  
   - El sistema debe proporcionar un display local para la visualización de datos y ajuste del controlador. Este display permitirá la configuración de las características del controlador.
     
4. Asegurar la escalabilidad y la adaptabilidad del sistema:
  - El sistema debe ser diseñado de tal manera que permita agregar nuevas funcionalidades y características en el futuro, manteniendo la facilidad de uso y la eficiencia en el control.

## **Desarrollo del Proyecto:**  

**Definición 1 - Entradas de Control:**  
Las entradas de control estarán compuestas por sensores resistivos, entradas analógicas (0-10 v; 0-20 ma; 4-20ma), entradas digitales (asociadas a funciones de hasta 5 variables digitales), y temporización para la entrada digital. Se implementará una función de anti-bounce para las entradas digitales, evitando la interpretación errónea de las señales. Las entradas analógicas contarán con la capacidad de realizar conversiones de señales analógicas a digitales para su procesamiento posterior.  

**Definición 2 - Salidas de Control:**  
Las salidas de control estarán compuestas por PWM, salida analógica (0-10v; 0-20ma; 4-20ma), y salida digital (cada una podrá definir una función lógica, cuyas variables son las DI definidas como tales). Se implementará la posibilidad de temporizar las funciones, y se añadirá la posibilidad de variar la frecuencia de la salida PWM en función de una entrada analógica, lo que permitirá controlar la velocidad de un motor, por ejemplo.  

**Definición 3 - Visualización y Ajuste:**  
La visualización de los datos y el ajuste del ControladorMx se llevarán adelante mediante un display local i2c, que se encargará de la configuración de las características del controlador. Esto incluirá la habilitación de entradas y salidas, la configuración del modo de operación, y la definición de las funciones lógicas para las salidas digitales en función de las entradas digitales. Además, se proporcionará una interfaz intuitiva para el ajuste de parámetros como la frecuencia del PWM, y la posibilidad de vincular entradas y salidas específicas. Se considerará la inclusión de un sistema de ayuda en pantalla para facilitar la configuración del controlador por parte_de_lusuario. 

**El ControladorMx se diseñará con un enfoque en la escalabilidad y la adaptabilidad, permitiendo la inclusión de nuevas funcionalidades en el futuro.**

## **Metodología de Desarrollo:**  
Para este trabajo práctico, utilizaremos una metodología ágil de desarrollo. Esto implica una serie de sprints, cada uno de los cuales produce una parte funcional del proyecto. Las metodologías ágiles promueven el desarrollo iterativo y el constante feedback, lo que permite a los equipos adaptarse rápidamente a los cambios y mejorar la eficiencia del proyecto.
