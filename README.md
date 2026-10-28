# SOLID-Inversion-Dependencias
Ejemplo en C++ del Principio de Inversión de Dependencias (DIP) de SOLID.

Este principio se implementa usando la clase abstracta EnvioRcibo para que la clase AdmProducto no dependa directamente de las clases de envio.
- EnvioRecibo.h define la interfaz de envío.
- EnviarEmail y EnviarApp heredan de EnvioRecibo y definen cómo enviar el recibo.
- AdmProducto.h usa un puntero EnvioRecibo* en su método Compra() para recibir cualquier tipo de envío.
