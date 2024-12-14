# FAM Hotel

¡Bienvenido a **FAM Hotel**! Esta es una aplicación móvil desarrollada para Android que implementa una arquitectura **MVVM** con **Firebase**. La app está orientada a la gestión de reservas en un hotel y otras funcionalidades clave como autenticación, subida de fotos, y actualizaciones en tiempo real.

---

## 🎯 **Características principales**
- **Autenticación Firebase**: Registro e inicio de sesión con **Firebase Authentication**.
- **Gestión de reservas**:  
  - Buscar y gestionar diferentes reservas, con diferentes tipos de alojamiento.  
- **Contratación de servicios**:
  - Permite la contratación de servicios que se vincularán a una reserva.
- **Subida de fotos**:  
  - Subir fotos de perfil al registrarse o actualizar desde el perfil.  
  - Manejo eficiente de imágenes con Firebase Storage.
- **Firestore en tiempo real**:  
  - Actualización dinámica de datos como comentarios, reservas y habitaciones disponibles.
- **Transacciones en Firestore**:  
  - Operaciones ACID para manejar múltiples documentos relacionados.
- **Arquitectura MVVM**:  
  - Uso de ViewModels, UseCases y Repositorios para desacoplar la lógica de negocio y la UI.

---

## 📂 **Estructura del proyecto**
La app sigue una organización de paquetes clara y modular basada en la arquitectura MVVM:

```plaintext
src/
├── data/          
		├── models/ 		#Modelo de datos
		├── repositories/ 		#Repositorios
├── domain/ 		# Casos de uso
├── ui/		# Interfaz gráfica
		├── mainActivity/ 		# Cada carpeta contiene los adapters, fragments y viewmodels correspondientes
				├── common/
				├── findroom/ 
				├── hotel/
				├── profile/
				├── reservas/
				├── servicios/
		├── startActivity/ 		# Fragments para el login y el registro


```

---

## 🛠️ **Requisitos técnicos**
- **SDK mínimo:** Android 6.0 (API 23)
- **Lenguaje principal:** Java
- **Dependencias clave:**
  - Firebase Authentication
  - Firebase Firestore
  - Firebase Storage
  - Material Components
  - Picasso (para manejo de imágenes)

---

## 📝 **¿Qué hace la app?**

### 1. **Autenticación**
La app permite a los usuarios registrarse y autenticarse con su correo electrónico y una contraseña segura. 


![autenticacion y registro](https://github.com/user-attachments/assets/d09572b5-0678-4f45-9b5e-e9d8da05adc0)
	

---
### 2. **Búsqueda de habitaciones**
Los usuarios pueden buscar habitaciones disponibles seleccionando una fecha.

![Búsqueda de habitaciones](https://github.com/user-attachments/assets/02536267-441a-4ee2-8999-fd1f691602c6)



---

### 3. **Contratación de servicios**
Los usuarios pueden contratar servicios para sus estancias.

![Pantalla de búsqueda de servicios](https://github.com/user-attachments/assets/ab5ce401-6a72-484e-95cc-04340337c0c9)



---

### 4. **Servicio de habitaciones**
Uno de los servicios que se ofrece es el servicio de habitaciones, donde los usuarios podrán solicitar artículos durante las 24 horas.

![Servicion de habitaciones](https://github.com/user-attachments/assets/d7649bf4-fa9f-4f00-a1c1-57f45443af25)

![Carta servicio de habitaciones](https://github.com/user-attachments/assets/0ac18c36-264a-4e47-819c-09f14cfc7122)

![Carta servicop de habitaciones 2](https://github.com/user-attachments/assets/22b04358-8d03-4156-bd32-2054a9846920)




### 5. **Detalles de la reserva**
Todos los detalles de la reserva, incluyendo una lista de servicios que se han ido contratando.

![Detalles de la reserva](https://github.com/user-attachments/assets/d8d74516-2b2c-46f4-a857-cfc5997f53df)


---

### 6. **Actualización de perfil**
Actualiza tu foto de perfil con una imagen subida desde la galería, modifica tu nombre o cualquier otra información.

![Pantalla de perfil](https://github.com/user-attachments/assets/da2fe706-01ec-49a3-adb3-99c5b9a7be7d)


---

### 7. **Visualización en tiempo real**
Los comentarios del servicio, las habitaciones disponibles y otros datos relevantes se actualizan en tiempo real gracias a Firestore y LiveData.

---


## 👨‍💻 **Contribuciones**
¡Las contribuciones son bienvenidas! Si tienes ideas para mejorar la app, siéntete libre de abrir un issue o enviar un pull request.

---

## 📄 **Licencia**
Este proyecto está licenciado bajo la [Apache 2.0 License](LICENSE).

---

