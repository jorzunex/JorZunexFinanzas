# 💰 JorZunexSolutions - Sistema de Finanzas

Sistema de gestión financiera para JorZunexSolutions (Jorge Andres Carmona Ramirez & Jose Manuel Zuluaga Figueroa).

## ✨ Características

- **Autenticación**: Dos usuarios con acceso completo
- **Paleta de Colores**: Diseño basado en JorZunex (neon cyan/blue, púrpura, gradientes)
- **Iconos Profesionales**: Phosphor Icons de alta calidad
- **Animaciones**: Efectos de entrada, transiciones suaves, partículas de fondo
- **Gráficos Interactivos**: Chart.js con gráficos de barras, dona y líneas
- **Sincronización Cloud**: Compatible con Supabase (configuración requerida)

---

## 🚀 Sincronización entre dispositivos

### Opción 1: Configurar Supabase (Recomendado)

Para sincronizar datos entre dispositivos, configura Supabase:

1. **Crea una cuenta** en [supabase.com](https://supabase.com) (gratis)
2. **Crea un nuevo proyecto** 
3. **Ve a Settings > API** y copia:
   - Project URL
   - anon / public key
4. **Crea la tabla** en SQL Editor:
```sql
CREATE TABLE finanzas (
  id SERIAL PRIMARY KEY,
  data JSONB NOT NULL,
  created_at TIMESTAMP WITH TIME ZONE DEFAULT NOW(),
  updated_at TIMESTAMP WITH TIME ZONE DEFAULT NOW()
);
-- Habilita Row Level Security para permitir lectura/escritura
ALTER TABLE finanzas ENABLE ROW LEVEL SECURITY;
CREATE POLICY "Allow all" ON finanzas FOR ALL USING (true) WITH CHECK (true);
```

5. **Edita el archivo index.html** y reemplaza:
```javascript
const SUPABASE_URL = 'https://TU_PROYECTO.supabase.co';
const SUPABASE_KEY = 'TU_KEY_AQUI';
```
Elimina el comentario de la línea `// const supabase = window.supabase...`

### Opción 2: Usar localStorage (Sin cloud)

Los datos se guardan en el navegador. Para compartir datos:
- Usa el botón **Exportar** para descargar un JSON
- El otro usuario puede Importar los datos (próximamente)

---

## 📱 Enlace de la App

**URL**: https://jorzunex.github.io/JorZunexFinanzas/

---

## 📋 Estructura de Datos

La app soporta:
- **Tipos**: Ingreso, Egreso, Ahorro, Otro
- **Categorías Ingresos**: Sueldo, Negocio, Deudas, Otro
- **Categorías Egresos**: Servicios, Gastos, Gastos Operativos, Nómina, Marketing
- **Campos**: Fecha, Categoría, Concepto, Presupuesto, Monto Real

---

## 🛠️ Tecnologías

- HTML5, CSS3, JavaScript
- Phosphor Icons
- Chart.js
- Supabase (opcional)
- GitHub Pages

---

**JorZunexSolutions** - *"Innovación · Software · Inteligencia Artificial"*