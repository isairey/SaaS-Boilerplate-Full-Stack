# 🚀 SaaS Boilerplate Full Stack

Una plantilla **Open Source** para desarrollar aplicaciones **SaaS** modernas, escalables y listas para producción.

Este proyecto proporciona una arquitectura completa para acelerar el desarrollo de plataformas web, incorporando autenticación, gestión de equipos, pagos, almacenamiento de archivos, notificaciones, colaboración en tiempo real y muchas otras funcionalidades esenciales.

---

# ✨ Características

- 🔐 Autenticación con Google OAuth
- 📧 Inicio de sesión Passwordless mediante correo electrónico
- 👥 Gestión de usuarios y equipos
- 💬 Sistema de discusiones y publicaciones
- 💳 Suscripciones y pagos con Stripe
- 📁 Subida y gestión de archivos con AWS S3
- 📨 Correos automáticos mediante AWS SES
- 📩 Integración con Mailchimp
- ⚡ Comunicación en tiempo real con Socket.IO
- 📊 Google Analytics
- 🔒 Seguridad con Helmet
- 🌐 Renderizado del lado del servidor (SSR)
- 📱 Diseño responsive
- ☁️ Arquitectura preparada para producción
- 🚀 Compatible con AWS, Heroku y Serverless

---

# 🏗️ Arquitectura del Proyecto

El proyecto está dividido en múltiples aplicaciones independientes:

| Aplicación | Descripción |
|------------|-------------|
| **App** | Interfaz web desarrollada con Next.js |
| **API** | Backend desarrollado con Express y TypeScript |
| **Lambda** | Funciones Serverless para AWS |
| **MongoDB** | Base de datos principal |
| **AWS S3** | Almacenamiento de archivos |
| **Stripe** | Sistema de pagos |
| **Google OAuth** | Autenticación social |

---

# 🛠 Tecnologías Utilizadas

### Frontend

- Next.js
- React
- TypeScript
- Material UI
- MobX

### Backend

- Node.js
- Express
- TypeScript
- MongoDB
- Mongoose

### Servicios

- Google OAuth
- Stripe
- AWS S3
- AWS SES
- Mailchimp
- Socket.IO
- Google Analytics

---

# 📂 Estructura del Proyecto

```
📦 SaaS-Boilerplate-Full-Stack
│
├── app/
│   ├── components/
│   ├── pages/
│   ├── server/
│   ├── public/
│   └── lib/
│
├── api/
│   ├── server/
│   ├── models/
│   ├── utils/
│   └── test/
│
├── lambda/
│
├── book/
│
└── README.md
```

---

# 🚀 Instalación

## 1. Clonar el repositorio

```bash
git clone https://github.com/isairey/SaaS-Boilerplate-Full-Stack.git
```

---

## 2. Entrar al proyecto

```bash
cd SaaS-Boilerplate-Full-Stack
```

---

## 3. Instalar dependencias

### Aplicación Web

```bash
cd app

yarn
```

### API

```bash
cd ../api

yarn
```

---

# ⚙ Variables de Entorno

El proyecto utiliza archivos `.env` para almacenar las credenciales necesarias.

## API

```env
MONGO_URL=

GOOGLE_CLIENTID=

GOOGLE_CLIENTSECRET=

AWS_ACCESSKEYID=

AWS_SECRETACCESSKEY=

AWS_REGION=

SESSION_SECRET=

SESSION_NAME=

MAILCHIMP_API_KEY=

STRIPE_TEST_SECRETKEY=

STRIPE_LIVE_SECRETKEY=

URL_APP=http://localhost:3000

URL_API=http://localhost:8000
```

## Aplicación

```env
NEXT_PUBLIC_URL_APP=http://localhost:3000

NEXT_PUBLIC_URL_API=http://localhost:8000

NEXT_PUBLIC_STRIPE_TEST_PUBLISHABLEKEY=

NEXT_PUBLIC_GA_MEASUREMENT_ID=
```

---

# ▶ Ejecutar el Proyecto

## Backend

```bash
cd api

yarn dev
```

Servidor:

```
http://localhost:8000
```

---

## Frontend

```bash
cd app

yarn dev
```

Aplicación:

```
http://localhost:3000
```

---

# 💳 Sistema de Pagos

El proyecto incorpora integración con **Stripe**, permitiendo:

- Suscripciones
- Actualización de métodos de pago
- Historial de pagos
- Webhooks
- Cancelación de suscripciones

---

# 👥 Gestión de Usuarios

El sistema permite:

- Registro de usuarios
- Inicio de sesión
- Inicio con Google
- Inicio Passwordless
- Gestión del perfil
- Cambio de información personal
- Administración de equipos
- Invitación de miembros
- Roles y permisos

---

# 💬 Sistema de Colaboración

Incluye funcionalidades para trabajo en equipo:

- Publicaciones
- Discusiones
- Comentarios
- Gestión de equipos
- Comunicación en tiempo real mediante Socket.IO

---

# 📂 Gestión de Archivos

Los usuarios pueden:

- Subir imágenes
- Eliminar archivos
- Administrar avatares
- Gestionar archivos de equipos

Todo el almacenamiento se realiza mediante **AWS S3**.

---

# 📧 Notificaciones

El sistema envía automáticamente correos electrónicos para:

- Bienvenida
- Invitaciones
- Confirmaciones
- Recuperación de acceso
- Pagos
- Suscripciones

Utilizando **AWS SES**.

---

# 🔐 Seguridad

La plataforma incorpora múltiples mecanismos de seguridad:

- OAuth 2.0
- Passwordless Login
- Sesiones seguras
- Helmet
- Cookies protegidas
- Variables de entorno
- Autenticación basada en sesiones

---

# 📊 Analítica

Integración con:

- Google Analytics
- Mailchimp
- Stripe Dashboard

---

# ☁ Despliegue

El proyecto puede desplegarse fácilmente en:

- AWS Elastic Beanstalk
- AWS Lambda
- Heroku
- Vercel
- Servidores propios

---

# 📷 Funcionalidades Principales

- 🔐 Inicio de sesión
- 👤 Gestión de usuarios
- 👥 Equipos
- 💬 Publicaciones
- 📝 Discusiones
- 📁 Subida de archivos
- 💳 Pagos
- 📊 Estadísticas
- 📧 Correos automáticos
- ☁ Almacenamiento en la nube
- ⚡ Comunicación en tiempo real

---

# 📈 Escalabilidad

La arquitectura está diseñada para soportar aplicaciones SaaS de producción gracias a:

- Separación entre Frontend y Backend
- Arquitectura modular
- Servicios independientes
- Integración con AWS
- Server Side Rendering
- API desacoplada
- Arquitectura Serverless

---

# 👨‍💻 Desarrollado con

- React
- Next.js
- Node.js
- Express
- MongoDB
- Mongoose
- TypeScript
- Material UI
- MobX
- Socket.IO
- Stripe
- AWS S3
- AWS SES
- Mailchimp
- Google OAuth

---

# 📄 Licencia

Este proyecto se distribuye bajo la licencia **MIT**, permitiendo su uso, modificación y distribución para proyectos personales y comerciales.

