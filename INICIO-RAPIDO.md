# 🚀 Guía de Inicio Rápido

## ✅ Proyecto Creado Exitosamente

Tu sitio web **Helenismo & Paz** está listo para ser personalizado y desplegado en GitHub Pages.

## 📋 Lo que se ha creado

### Páginas
- ✅ **Inicio** (`index.astro`) - Hero con introducción y escuelas filosóficas
- ✅ **Blog** (`blog.astro`) - Artículo completo sobre helenismo y paz
- ✅ **Línea de Tiempo** (`timeline.astro`) - 30+ filósofos con tarjetas interactivas
- ✅ **Referencias** (`referencias.astro`) - Bibliografía académica completa

### Componentes
- ✅ **Header** - Navegación sticky con logo
- ✅ **Footer** - Información académica y enlaces
- ✅ **Timeline** - Carrusel interactivo con navegación
- ✅ **TimelineCard** - Tarjetas expandibles para cada filósofo

### Estilos
- ✅ Diseño inspirado en zed.dev
- ✅ 6 colores para escuelas filosóficas
- ✅ Totalmente responsive
- ✅ Animaciones suaves

### Configuración
- ✅ GitHub Actions para despliegue automático
- ✅ Configuración para GitHub Pages
- ✅ .gitignore configurado

## 🎬 Primeros Pasos

### 1. Probar Localmente

```bash
# Ya estás en el directorio correcto
npm run dev
```

Abre http://localhost:4321 en tu navegador.

### 2. Personalizar Información

**Archivo: `src/components/Footer.astro`**
```astro
Línea 12: <p><strong>Autor:</strong> [Tu Nombre Completo]</p>
Línea 35: <a href="https://github.com/[tu-usuario]/helenismo-paz">
```

**Archivo: `src/pages/blog.astro`**
```astro
Línea 16: <p class="author-name"><strong>[Tu Nombre Completo]</strong></p>
```

### 3. Añadir Fotos

**Foto del autor:**
- Reemplaza `public/images/author.jpg`
- Tamaño recomendado: 150x150px

**Fotos de filósofos (opcional):**
- Añade imágenes en `public/images/philosophers/`
- Actualiza referencias en `src/components/Timeline.astro`

### 4. Configurar GitHub Pages

**Archivo: `astro.config.mjs`**
```javascript
site: 'https://[tu-usuario-github].github.io',
base: '/helenismo-paz',  // O el nombre que elijas para tu repo
```

### 5. Crear Repositorio

```bash
# Inicializar Git (si no está inicializado)
git init

# Añadir archivos
git add .
git commit -m "Initial commit: Helenismo & Paz"

# Conectar con GitHub
git remote add origin https://github.com/[tu-usuario]/helenismo-paz.git
git branch -M main
git push -u origin main
```

### 6. Activar GitHub Pages

1. Ve a tu repositorio en GitHub
2. **Settings** → **Pages**
3. En "Build and deployment":
   - Source: **GitHub Actions**
4. El workflow se ejecutará automáticamente
5. Tu sitio estará en: `https://[tu-usuario].github.io/helenismo-paz`

## 🎨 Características Destacadas

### Línea de Tiempo Interactiva
- ✨ 30+ filósofos del helenismo
- 🎯 Navegación con flechas o teclado
- 📊 Barra de progreso
- 🎨 Código de colores por escuela
- 📱 Responsive

### Blog Académico
- 📝 ~2000 palabras sobre helenismo y paz
- 🏛️ 6 escuelas filosóficas analizadas
- 🕊️ Aplicación a construcción de paz
- 📚 Bien estructurado y referenciado

### Diseño Profesional
- 🎨 Inspirado en zed.dev
- ⚡ Rápido y optimizado
- 📱 Mobile-first
- ♿ Accesible

## 📝 Comandos Útiles

```bash
npm run dev          # Servidor de desarrollo
npm run build        # Build para producción  
npm run preview      # Vista previa del build
```

## 🔧 Personalización Avanzada

### Modificar Colores

**Archivo: `src/styles/global.css`**
```css
:root {
  --color-accent: #4f46e5;        /* Color principal */
  --color-cynicism: #f59e0b;      /* Cinismo */
  --color-epicureanism: #10b981;  /* Epicureísmo */
  --color-stoicism: #3b82f6;      /* Estoicismo */
  --color-skepticism: #8b5cf6;    /* Escepticismo */
  --color-eclecticism: #ec4899;   /* Eclecticismo */
  --color-neoplatonism: #ef4444;  /* Neoplatonismo */
}
```

### Añadir Más Filósofos

**Archivo: `src/components/Timeline.astro`**
```javascript
const philosophers = [
  // Añade tu filósofo aquí
  {
    name: 'Nombre del Filósofo',
    dates: 'XXX-YYY a.C.',
    school: 'Estoicismo',  // O la escuela correspondiente
    concepts: ['Concepto 1', 'Concepto 2'],
    peaceUtility: 'Explicación de su relevancia para la paz...'
  },
  // ...
];
```

### Editar Contenido del Blog

**Archivo: `src/pages/blog.astro`**

El contenido está en secciones `<section>`. Edita libremente manteniendo la estructura HTML.

## 📚 Documentación Adicional

- 📖 **README.md** - Información general del proyecto
- 📋 **INSTRUCCIONES.md** - Guía detallada de personalización
- 🌐 [Documentación de Astro](https://docs.astro.build)
- 📄 [GitHub Pages Docs](https://docs.github.com/pages)

## ✨ Próximos Pasos

1. ✅ Prueba el sitio localmente
2. ✅ Personaliza tu información
3. ✅ Añade tus fotos
4. ✅ Configura GitHub
5. ✅ Despliega tu sitio
6. ✅ Comparte tu trabajo

## 🎓 Información del Proyecto

**Universidad:** UNAD  
**Programa:** Filosofía  
**Asignatura:** Filosofía Antigua  
**Periodo:** 2025-1

## 💡 ¿Necesitas Ayuda?

- 📖 Consulta **INSTRUCCIONES.md** para detalles
- 🐛 Revisa la sección Troubleshooting
- 💬 Consulta la documentación de Astro
- 📧 Contacta a tu profesor

---

¡Tu sitio está listo! 🎉 Ahora solo necesitas personalizarlo y desplegarlo.
