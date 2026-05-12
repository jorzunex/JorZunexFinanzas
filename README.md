# 💰 JorZunexSolutions - Sistema de Finanzas

Sistema de gestión financiera para JorZunexSolutions (Jorge Andres Carmona Ramirez & Jose Manuel Zuluaga Figueroa).

## ✨ Características

- **Autenticación**: Dos usuarios con acceso completo
- **Paleta de Colores**: Diseño basado en JorZunex (neon cyan/blue, púrpura, gradientes)
- **Iconos Profesionales**: Phosphor Icons de alta calidad
- **Animaciones**: Efectos de entrada, transiciones suaves, partículas de fondo
- **Gráficos Interactivos**: Chart.js con gráficos de barras, dona y líneas
- **Sincronización**: Los datos se guardan en el navegador local (localStorage)
- **Acceso Mundial**: Al desplegar en GitHub Pages, ambos usuarios pueden acceder desde cualquier parte del mundo

## 🚀 Cómo Desplegar en GitHub Pages

### Paso 1: Crear Repositorio en GitHub

1. Ve a [GitHub](https://github.com) e inicia sesión
2. Haz clic en **"New repository"** (botón verde)
3. Repository name: `JorZunexFinanzas`
4. Visibility: **Public**
5. No inicialices con README (dejaremos los archivos que ya tenemos)
6. Haz clic en **"Create repository"**

### Paso 2: Subir los Archivos

En tu terminal, ejecuta estos comandos dentro de la carpeta `JorZunexFinanzas`:

```bash
cd ProyectosJorZunex/JorZunexFinanzas
git init
git add .
git commit -m "Initial commit - JorZunex Finances App"
```

Agrega el repositorio remoto (reemplaza `tu-usuario` con tu nombre de usuario):

```bash
git remote add origin https://github.com/tu-usuario/JorZunexFinanzas.git
```

Sube los archivos:

```bash
git push -u origin main
```

### Paso 3: Configurar GitHub Pages

1. Ve a tu repositorio en GitHub
2. Haz clic en **Settings** (Configuración)
3. En el menú izquierdo, ve a **Pages**
4. En "Build and deployment":
   - **Source**: Deploy from a branch
   - **Branch**: main (o master)
   - **Folder**: / (root)
5. Haz clic en **Save**

### Paso 4: Obtener tu URL

1. Espera 1-2 minutos mientras GitHub construye el sitio
2. Refresca la página de Settings > Pages
3. Verás un mensaje verde con la URL:
   ```
   Your site is live at https://tu-usuario.github.io/JorZunexFinanzas/
   ```

### 🌐 Enlace de JorZunexSolutions

**URL Final**: `https://jorzunex.github.io/JorZunexFinanzas/`

(Este enlace funciona porque el usuario del repositorio es `jorzunex`)

---

## 📱 Cómo Usar la App

1. **Accede** desde el enlace de GitHub Pages
2. **Selecciona** tu usuario (Jorge o Jose)
3. **Registra** ingresos y egresos
4. **Administra** cuentas por cobrar y pagar
5. **Consulta** reportes y gráficos
6. **Exporta** datos cuando necesites respaldos

### Notas sobre la Sincronización

- **Mismo navegador**: Si ambos usan el mismo navegador, los datos se comparten automáticamente via localStorage
- **Diferentes navegadores**: Cada navegador tiene su propio localStorage. Para sincronizar, pueden exportar/importar datos periódicamente
- **Solución Cloud**: Para sincronización real en tiempo real entre diferentes dispositivos, se necesitaría integrar Firebase, Supabase o un backend

---

## 🛠️ Tecnologías Usadas

- **HTML5** - Estructura
- **CSS3** - Estilos con variables CSS y animaciones
- **JavaScript** - Lógica y localStorage
- **Phosphor Icons** - Iconos profesionales
- **Chart.js** - Gráficos interactivos
- **GitHub Pages** - Hosting gratuito

---

## 📄 Estructura de Archivos

```
JorZunexFinanzas/
├── index.html    (Aplicación completa)
├── .nojekyll     (Para GitHub Pages)
└── README.md     (Este archivo)
```

---

**JorZunexSolutions** - *"Innovación · Software · Inteligencia Artificial"*