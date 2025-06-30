# 🌳 ArborVitae Scheduler - Sistema de Turnos UTN

Sistema completo de gestión de turnos para la UTN Facultad Regional San Francisco, desarrollado como parte del Trabajo Práctico de Diseño de Sistemas de Información.

## 🚀 Demo en Vivo

- **Frontend**: [https://arborvitae-scheduler.vercel.app/](https://arborvitae-scheduler.vercel.app/)
- **Backend API**: [https://backend-dsi.onrender.com](https://backend-dsi.onrender.com)

## 🌐 Deployment

### Frontend (Vercel)

- Deployment automático desde GitHub
- Variables de entorno configuradas en Vercel Dashboard
- Dominio personalizado: `arborvitae-scheduler.vercel.app`

### Backend (Render)

- Deployment automático desde GitHub
- Variables de entorno configuradas en Render Dashboard
- URL de producción: `backend-dsi.onrender.com`

## 🚀 Instalación y Desarrollo

### Prerrequisitos

- Node.js 18+
- npm o yarn
- Git

### 1. Clonar el repositorio con submódulos

```bash
git clone --recursive https://github.com/Ulises-Araya/TP-Diseno-de-Sistemas-New.git
cd TP-Diseno-de-Sistemas-New/Implementación
```

### 2. Instalar dependencias

```bash
# Instalar dependencias del proyecto principal
npm install

# Instalar dependencias del frontend
cd Frontend-DSI
npm install
cd ..

# Instalar dependencias del backend
cd Backend-DSI
npm install
cd ..
```

### 3. Configurar variables de entorno

#### Frontend (.env.local)

```env
NEXT_PUBLIC_SUPABASE_URL=tu_supabase_url
NEXT_PUBLIC_SUPABASE_ANON_KEY=tu_supabase_anon_key
NEXT_PUBLIC_API_URL=http://localhost:3001
```

#### Backend (.env)

```env
SUPABASE_URL=tu_supabase_url
SUPABASE_KEY=tu_supabase_service_key
JWT_SECRET=tu_jwt_secret
PORT=3001
```

### 4. Ejecutar en modo desarrollo

```bash
# Ejecutar frontend y backend simultáneamente
npm run dev

# O ejecutar individualmente
npm run dev --prefix Frontend-DSI  # Frontend en puerto 3000
npm run dev --prefix Backend-DSI   # Backend en puerto 3001
```
