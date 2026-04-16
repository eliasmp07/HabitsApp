# HabitsApp

![Status](https://img.shields.io/badge/Status-En%20Desarrollo-orange?style=for-the-badge)
![Kotlin](https://img.shields.io/badge/Kotlin-1.9.23-purple?style=for-the-badge&logo=kotlin)
![Android](https://img.shields.io/badge/Platform-Android-3DDC84?style=for-the-badge&logo=android)

**HabitsApp** es una aplicación de gestión de hábitos diseñada bajo una estrategia **OfflineFirst**, garantizando que las funcionalidades clave estén disponibles siempre, incluso sin conexión a internet. La arquitectura se basa en **Clean Architecture**, el patrón de diseño **MVVM**, y los principios **SOLID**, utilizando las herramientas más actuales del ecosistema Android.

---

## 📸 Screenshots

### Onboarding
| Paso 1 | Paso 2 | Paso 3 | Paso 4 |
| :---: | :---: | :---: | :---: |
| ![Onboarding 1](https://github.com/EliasMP07/HabitsApp/blob/master/app/src/main/assets/onboarding1.png) | ![Onboarding 2](https://github.com/EliasMP07/HabitsApp/blob/master/app/src/main/assets/onboarding2.png) | ![Onboarding 3](https://github.com/EliasMP07/HabitsApp/blob/master/app/src/main/assets/onboarding3.png) | ![Onboarding 4](https://github.com/EliasMP07/HabitsApp/blob/master/app/src/main/assets/onboarding4.png) |

### Core & Auth
| Login | Registro | Listado | Gestión |
| :---: | :---: | :---: | :---: |
| ![Login](https://github.com/EliasMP07/HabitsApp/blob/master/app/src/main/assets/authenticationlogin.png) | ![Register](https://github.com/EliasMP07/HabitsApp/blob/master/app/src/main/assets/authenticationregister.png) | ![Home](https://github.com/EliasMP07/HabitsApp/blob/master/app/src/main/assets/home_habits.png) | ![Create](https://github.com/EliasMP07/HabitsApp/blob/master/app/src/main/assets/home_create_habit.png) |

---

## ✨ Características Principales

* 🚀 **Estrategia OfflineFirst:** Acceso y edición de hábitos sin conexión mediante Room.
* 🔐 **Autenticación:** Gestión segura de usuarios con FirebaseAuth.
* 🔄 **Sincronización:** Persistencia en tiempo real con Firebase Realtime Database.
* ⏰ **Recordatorios:** Sistema de alertas persistentes usando `AlarmManager` y `WorkManager`.
* 🎨 **UI Moderna:** Interfaces reactivas con Jetpack Compose y Material Design 3.

---

## 🛠️ Stack Tecnológico

| Herramienta | Badge |
| :--- | :--- |
| **Lenguaje** | ![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?style=flat&logo=kotlin&logoColor=white) |
| **UI** | ![Compose](https://img.shields.io/badge/Jetpack_Compose-4285F4?style=flat&logo=jetpackcompose&logoColor=white) |
| **Local Storage** | ![Room](https://img.shields.io/badge/Room_DB-3DDC84?style=flat&logo=android&logoColor=white) |
| **Cloud** | ![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=flat&logo=firebase&logoColor=black) |
| **Inyección** | ![Hilt](https://img.shields.io/badge/Hilt-DA282A?style=flat&logo=android&logoColor=white) |
| **Async** | ![Coroutines](https://img.shields.io/badge/Coroutines-181717?style=flat&logo=kotlin&logoColor=white) |

---

## 🚀 Requisitos e Instalación

### Requisitos previos
* Android Studio Iguana
* Gradle Versión 8.3
* Kotlin 1.9.23 o superior

### Instalación
1.  Clona el repositorio:
    ```bash
    git clone [https://github.com/EliasMP07/HabitsApp.git](https://github.com/EliasMP07/HabitsApp.git)
    ```
2.  Importa el proyecto en Android Studio.
3.  Agrega tu archivo `google-services.json` de Firebase en la carpeta `app/`.
4.  Sincroniza Gradle y ejecuta en tu dispositivo/emulador.

---

## 📂 Estructura del Proyecto (Modular)

La aplicación utiliza un sistema de módulos para desacoplar responsabilidades:

- **`:core`**: Funcionalidades compartidas y componentes UI base.
- **`:authentication`**: Gestión de usuarios, repositorios de sesión y validaciones.
- **`:home`**: Módulo central de hábitos, base de datos local y lógica de alarmas.
- **`:onboarding`**: Pantallas de introducción y gestión de `DataStore` para estados de primer inicio.
- **`:settings`**: Configuración de perfil y utilidades de cuenta.
- **`:navigation`**: Grafo de navegación centralizado y rutas.

---

## 🤝 Contribución

¡Este proyecto está abierto a contribuciones! Si quieres ayudar a mejorarlo, sigue estos pasos:

1. **Haz un Fork** del proyecto.
2. **Crea una rama** para tu mejora (`git checkout -b feature/NuevaFuncionalidad`).
3. **Realiza tus cambios** y haz un **Commit** descriptivo (`git commit -m 'Añadida funcionalidad X'`).
4. **Sube tus cambios** (`git push origin feature/NuevaFuncionalidad`).
5. **Abre un Pull Request** explicando tus cambios detalladamente.

Cualquier sugerencia sobre la arquitectura o nuevas librerías es bienvenida.

---

## 📄 Licencia

Este proyecto es distribuido bajo la licencia **MIT**. Siéntete libre de usarlo, editarlo y compartirlo.
