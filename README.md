# 🏋️ App Virtual Personal Trainer

<div align="center">

![React Native](https://img.shields.io/badge/React_Native-0.79.6-61DAFB?style=for-the-badge&logo=react&logoColor=white)
![Expo](https://img.shields.io/badge/Expo-53.0-000020?style=for-the-badge&logo=expo&logoColor=white)
![Firebase](https://img.shields.io/badge/Firebase-12.2-FFCA28?style=for-the-badge&logo=firebase&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-5.8-3178C6?style=for-the-badge&logo=typescript&logoColor=white)


**Una aplicación móvil que actúa como tu entrenador personal virtual — rutinas, seguimiento y motivación en tu bolsillo.**

[📱 Descargar APK](https://expo.dev/accounts/milo1027/projects/EntrenadorPersonal/builds/dbfe1a98-583c-4187-bd55-25544502c64c) · [🐛 Reportar Bug](https://github.com/DreyRo/App-Virtual-Personal-Trainer/issues) · [💡 Solicitar Feature](https://github.com/DreyRo/App-Virtual-Personal-Trainer/issues)

</div>

---

## 📋 Tabla de Contenidos

- [Sobre el Proyecto](#-sobre-el-proyecto)
- [Funcionalidades](#-funcionalidades)
- [Tecnologías](#-tecnologías)
- [Estructura del Proyecto](#-estructura-del-proyecto)
- [Requisitos Previos](#-requisitos-previos)
- [Instalación](#-instalación)
- [Variables de Entorno](#-variables-de-entorno)
- [Uso](#-uso)
- [Equipo](#-equipo)

---

## 🎯 Sobre el Proyecto

**App Virtual Personal Trainer** es una aplicación móvil desarrollada con **React Native + Expo** que permite a los usuarios seguir rutinas de entrenamiento personalizadas, registrar su progreso y mantenerse motivados sin necesidad de un entrenador físico presencial.

La app utiliza **Firebase** como backend para autenticación y almacenamiento de datos, y **SQLite** para persistencia local, lo que permite usarla incluso sin conexión a internet.

---

## ✨ Funcionalidades

- 🔐 **Autenticación** — registro e inicio de sesión con Firebase Auth
- 🏃 **Rutinas de entrenamiento** — biblioteca de ejercicios con instrucciones
- 📊 **Seguimiento de progreso** — gráficas de rendimiento con Chart Kit
- 🎵 **Audio y video** — reproducción de guías en audio/video dentro de la app
- 📷 **Galería** — selección de imágenes con el picker nativo
- 🌐 **Modo offline** — datos locales con SQLite + sincronización con Firebase
- 📱 **Navegación fluida** — stack y tabs con React Navigation

---

## 🛠️ Tecnologías

| Categoría | Tecnología |
|-----------|-----------|
| Framework | React Native 0.79 + Expo SDK 53 |
| Lenguaje | JavaScript / TypeScript |
| Backend / Auth | Firebase 12 |
| Base de datos local | expo-sqlite + react-native-sqlite-storage |
| Navegación | React Navigation (Stack + Bottom Tabs) |
| Multimedia | expo-av, expo-audio, expo-video |
| Gráficas | react-native-chart-kit + react-native-svg |
| Iconos | @expo/vector-icons |
| Linter | ESLint + eslint-config-expo |

---

## 📁 Estructura del Proyecto

```
App-Virtual-Personal-Trainer/
├── assets/
│   └── images/          # Recursos gráficos de la app
├── context/             # Context API — estado global
├── data/                # Datos estáticos (ejercicios, rutinas, etc.)
├── navigation/          # Configuración de React Navigation
├── screens/             # Pantallas de la aplicación
├── .vscode/             # Configuración del editor
├── android/             # Código nativo Android (generado por Expo)
├── App.js               # Punto de entrada principal
├── firebaseConfig.js    # Configuración de Firebase (usar .env)
├── app.json             # Configuración de Expo
├── eas.json             # Configuración de EAS Build
└── package.json
```

---

## ✅ Requisitos Previos

Antes de instalar, asegúrate de tener:

- [Node.js](https://nodejs.org/) v18 o superior
- [npm](https://www.npmjs.com/) o [Yarn](https://yarnpkg.com/)
- [Expo CLI](https://docs.expo.dev/get-started/installation/) instalado globalmente
- [Expo Go](https://expo.dev/client) en tu dispositivo móvil (para pruebas rápidas)
- Una cuenta en [Firebase](https://firebase.google.com/) con un proyecto creado

```bash
# Instalar Expo CLI globalmente
npm install -g expo-cli
```

---

## 🚀 Instalación

1. **Clona el repositorio**
```bash
git clone https://github.com/DreyRo/App-Virtual-Personal-Trainer.git
cd App-Virtual-Personal-Trainer
```

2. **Cambia a la rama del grupo**
```bash
git checkout grupo5
```

3. **Instala las dependencias**
```bash
npm install
# o con yarn
yarn install
```

4. **Configura las variables de entorno** (ver sección siguiente)

5. **Inicia la aplicación**
```bash
npx expo start
```

6. **Abre la app** en Expo Go escaneando el QR, o en un emulador Android/iOS.

---

## 🔐 Variables de Entorno

Crea un archivo `.env` en la raíz del proyecto basándote en `.env.example`:

```bash
cp .env.example .env
```

> ⚠️ **Nunca subas tu archivo `.env` al repositorio.** Está incluido en `.gitignore`.

Llena las variables con los datos de tu proyecto Firebase:

```env
FIREBASE_API_KEY=tu_api_key
FIREBASE_AUTH_DOMAIN=tu_proyecto.firebaseapp.com
FIREBASE_PROJECT_ID=tu_proyecto_id
FIREBASE_STORAGE_BUCKET=tu_proyecto.appspot.com
FIREBASE_MESSAGING_SENDER_ID=tu_sender_id
FIREBASE_APP_ID=tu_app_id
```

Puedes obtener estos valores desde la consola de Firebase → **Configuración del proyecto → Tu app**.

---

## 📱 Uso

### Correr en Android
```bash
npx expo run:android
```

### Correr en iOS
```bash
npx expo run:ios
```

### Correr en Web
```bash
npx expo start --web
```

### Linter
```bash
npm run lint
```

### Build con EAS
```bash
eas build --platform android
```

---

## 📲 APK disponible

Puedes descargar e instalar directamente la APK compilada:

👉 [Descargar APK desde Expo](https://expo.dev/accounts/milo1027/projects/EntrenadorPersonal/builds/dbfe1a98-583c-4187-bd55-25544502c64c)

---

## 👥 Equipo

| Nombre           | GitHub                                       |
|------------------|----------------------------------------------|
| Andrey           | [@DreyRo](https://github.com/DreyRo)         |
| brahianxcx       | [@brahianxcx](https://github.com/brahianxcx) |
| Camilo Jaramillo | [@Milo1027 ](https://github.com/Milo1027)    |
