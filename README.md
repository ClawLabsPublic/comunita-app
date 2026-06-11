# Comunita.app

> La forma más inteligente de gestionar comunidades de vecinos

## Overview
Comunita.app es una aplicación web moderna diseñada para simplificar la gestión de comunidades de vecinos. Construida con React 19, TypeScript y Vite, ofrece una experiencia rápida y fluida tanto en escritorio como en móvil gracias a su soporte PWA completo con service worker y manifest.

## How it works
La aplicación utiliza React Context para la gestión del estado global, permitiendo cambiar entre múltiples comunidades de vecinos con el componente `CommunitySwitcher`. Los datos se persisten en `localStorage` en modo demo, mientras que la integración con **Supabase** está preparada para producción con autenticación y base de datos en la nube. La UI está construida sobre **Tailwind CSS 3.4** y **shadcn/ui** con componentes Radix UI accesibles, garantizando modales, diálogos y menús sin problemas de z-index o stacking context.

## Use cases
- **Administradores de fincas** que gestionan múltiples edificios y urbanizaciones desde un único panel.
- **Presidentes de comunidad** que necesitan controlar viviendas, vecinos y comunicaciones internas.
- **Vecinos** que acceden a información de su comunidad, convocatorias y documentos.
- **Empresas de gestión** que buscan una solución multi-tenant escalable con roles Super Admin y Admin de Comunidad.

El proyecto está desplegado en **Vercel** con CI/CD automático conectado al repositorio GitHub, facilitando iteraciones rápidas y despliegues instantáneos tras cada push.

[🌐 Live site](https://comunita.app/) · [📄 Project page](https://clawlabs.site/projects/comunita-app)

## Features
- Gestión multi-comunidad con CommunitySwitcher
- Roles de usuario: Super Admin y Admin de Comunidad
- PWA con service worker, manifest y splash screens
- Integración preparada con Supabase para backend en la nube
- UI accesible con shadcn/ui y Radix UI
- Demo mode con localStorage sin necesidad de backend

## Tech stack
`React 19` `TypeScript` `Vite` `Tailwind CSS` `shadcn/ui` `Radix UI` `Supabase` `React Context` `PWA` `Vitest` `Playwright` `ESLint`

## FAQ

### ¿Cómo puedo probar Comunita.app sin registrarme?
Puedes acceder al modo demo usando el email `demo@comunita.app` con cualquier contraseña. Tendrás acceso completo como Super Admin a tres comunidades de prueba con datos precargados en localStorage.

### ¿Comunita.app funciona en móvil como una app nativa?
Sí, Comunita.app es una Progressive Web App (PWA) con service worker y manifest configurados. Puedes instalarla desde el navegador en iOS o Android y usarla como una app nativa con acceso desde la pantalla de inicio.

### ¿Qué tecnologías usa Comunita.app por debajo?
Está construida con React 19, TypeScript y Vite como bundler. La UI usa Tailwind CSS 3.4 y shadcn/ui con componentes Radix UI. El backend está integrado con Supabase para autenticación y base de datos en la nube.

### ¿Puedo gestionar varios edificios o comunidades desde un mismo panel?
Sí, la versión 3.0 introduce soporte multi-comunidad completo. El componente CommunitySwitcher permite cambiar entre comunidades activas y todos los datos, filtros y vistas se actualizan automáticamente según la comunidad seleccionada.

### ¿Cómo se despliega Comunita.app en producción?
El proyecto está desplegado en Vercel con CI/CD automático conectado al repositorio GitHub. Cada push a la rama `main` genera un despliegue automático. Solo necesitas configurar las variables de entorno de Supabase en el panel de Vercel.

### ¿Es posible usar Comunita.app sin conexión a internet?
En modo demo, los datos se almacenan en localStorage y la PWA puede funcionar parcialmente sin conexión gracias al service worker. Para producción con Supabase, se requiere conexión para sincronizar datos en tiempo real.

---

_Project info maintained with [ClawLabs](https://clawlabs.site/projects/comunita-app) — an AI-first project manager for vibe coding._
