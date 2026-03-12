# 📊 Aplicación Web IMC - Java EE

Proyecto final de **Computación Avanzada en Java**  
Autora: **Laly Zamitiz Bonilla**

---

## 📌 Descripción
Esta aplicación web permite calcular el **Índice de Masa Corporal (IMC)** de los usuarios, almacenar sus registros y mostrar un historial.  
El IMC es un valor numérico utilizado por la OMS para evaluar si una persona tiene un peso saludable en relación con su estatura.

**Fórmula:**

---

## 🏗️ Arquitectura (MVC)
El proyecto sigue el patrón **Modelo-Vista-Controlador (MVC)** usando **Java EE, Servlets y JSP**.

### 🔹 Modelos
- **Usuario**: Datos personales (nombre, username, contraseña, edad, sexo, estatura).
- **RegistroIMC**: Cálculo específico (peso, valor del IMC, fecha) asociado a un usuario.

### 🔹 Vistas (JSP)
- `index.jsp`: Inicio de sesión y registro.
- `dashboard.jsp`: Pantalla principal con cálculo de IMC e historial.
- `perfil.jsp`: Información del usuario.
- `historial.jsp`: Registros previos de IMC.

### 🔹 Controladores (Servlets)
- **AuthServlet**: Procesa login y registro.
- **IMCServlet**: Recibe el peso, calcula el IMC y guarda el resultado.

### 🔹 Acceso a Datos (DAO)
- **UsuarioDAO**: Manejo de datos de usuarios.
- **IMCDAO**: Manejo de registros de IMC.

---

## 🗄️ Base de Datos
La aplicación utiliza una base de datos relacional con las siguientes tablas:

- **Usuarios**: Información personal y credenciales.
- **RegistrosIMC**: Peso, IMC calculado y fecha, vinculados al usuario.

---

## 🎨 Interfaces de Usuario
- **Login**: Acceso al sistema.
- **Register**: Registro de nuevos usuarios.
- **Dashboard**: Cálculo de IMC y visualización de resultados.
- **Historial**: Lista de registros anteriores.
- **Perfil**: Datos del usuario.

---

## 🚀 Tecnologías Utilizadas
- Java EE (Servlets, JSP)
- JDBC (Data Access Objects)
- HTML, CSS, Bootstrap (Frontend)
- MySQL (Base de Datos)

---

## 📂 Estructura del Proyecto

---

## ✅ Funcionalidades
- Registro e inicio de sesión de usuarios.
- Cálculo automático del IMC.
- Almacenamiento de registros en base de datos.
- Visualización de historial de IMC.
- Gestión de perfil de usuario.

---

## 📌 Próximos Pasos
- Implementar validaciones más robustas.
- Agregar gráficos para visualizar evolución del IMC.
- Mejorar seguridad con cifrado de contraseñas.
