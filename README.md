# Sistema de vuelos

Programa que busca gestionar la programación de vuelos para los usuarios (administrador de la aerolínea) a través de una interfaz simple en código que permite:

- Registrar aviones.
- Programar vuelos.
- Mostrar vuelos programados.
- Cancelar vuelos.

El sistema se compone de tres clases principales: **Avión**, **Vuelo** y **SistemaFBO**.

---

## Flujo general del programa:

1. El administrador registra uno o más aviones.
2. Programa vuelos seleccionando un avión registrado y especificando los detalles del vuelo.
3. Puede consultar los vuelos programados en cualquier momento.
4. Si es necesario, puede cancelar un vuelo.

---

## Relaciones para el diagrama de clases:

### **Relación entre Avión y Vuelo**
- Relación de **agregación**: un vuelo utiliza un avión, pero el avión no depende del vuelo.

### **Relación entre SistemaFBO con Vuelo y Avión**
- Relación de **composición**: `SistemaFBO` contiene listas de instancias de las clases `Avion` y `Vuelo`.

---

## Estructura del proyecto:

El programa está diseñado para ser ejecutado desde la consola con interacción directa del usuario. Las tres clases principales están organizadas como sigue:

### 1. **Avión**
Representa un avión en el sistema, con atributos como matrícula, modelo, capacidad de pasajeros y capacidad de carga.

### 2. **Vuelo**
Representa un vuelo programado, asociando un avión con una ruta específica y un horario.

### 3. **SistemaFBO**
Gestiona las funcionalidades principales:
- Registro de aviones.
- Programación de vuelos.
- Visualización de vuelos.
- Cancelación de vuelos.
