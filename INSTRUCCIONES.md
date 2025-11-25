# Instrucciones de Personalización

## Pasos para Personalizar el Sitio

### 1. Actualizar Información Personal

#### Footer (src/components/Footer.astro)
Busca y reemplaza:
```astro
<p><strong>Autor:</strong> [Tu Nombre Completo]</p>
```

Actualiza también el link del repositorio GitHub:
```astro
<a href="https://github.com/[tu-usuario]/helenismo-paz">
```

#### Blog (src/pages/blog.astro)
Actualiza la información del autor:
```astro
<p class="author-name"><strong>[Tu Nombre Completo]</strong></p>
```

### 2. Añadir Foto del Autor

Reemplaza el archivo `public/images/author.jpg` con tu foto (recomendado: 150x150px, formato circular).

### 3. Añadir Imágenes de Filósofos

Coloca imágenes de filósofos en `public/images/philosophers/` con el formato:
- Tamaño: 200x200px
- Formato: PNG o JPG
- Nombres sugeridos: `antisthenes.png`, `diogenes.png`, `epicuro.png`, etc.

Luego actualiza las referencias en `src/components/Timeline.astro`:
```javascript
{
  name: 'Antístenes',
  imagePlaceholder: '/images/philosophers/antisthenes.png',
  // ... resto de propiedades
}
```

### 4. Configurar para GitHub Pages

#### Actualizar astro.config.mjs
```javascript
export default defineConfig({
  site: 'https://[tu-usuario-github].github.io',
  base: '/helenismo-paz',
});
```

#### Crear Repositorio en GitHub
```bash
# Inicializar repositorio
git init
git add .
git commit -m "Initial commit: Helenismo & Paz website"

# Conectar con GitHub
git remote add origin https://github.com/[tu-usuario]/helenismo-paz.git
git branch -M main
git push -u origin main
```

#### Activar GitHub Pages
1. Ve a tu repositorio en GitHub
2. Settings → Pages
3. En "Build and deployment", selecciona "GitHub Actions" como fuente
4. El sitio se desplegará automáticamente

### 5. Personalizar Contenido del Blog

Edita `src/pages/blog.astro` para:
- Actualizar fechas
- Modificar o ampliar el contenido filosófico
- Añadir tus propias reflexiones

### 6. Actualizar Referencias

Edita `src/pages/referencias.astro` para:
- Añadir nuevas referencias bibliográficas
- Actualizar fechas de acceso a recursos en línea
- Añadir obras que hayas consultado

## Comandos Útiles

```bash
# Desarrollo
npm run dev           # Servidor local en http://localhost:4321

# Build
npm run build         # Construir sitio estático

# Vista previa
npm run preview       # Ver build local antes de desplegar

# Limpiar cache
rm -rf node_modules .astro dist
npm install
```

## Troubleshooting

### El sitio no carga correctamente en GitHub Pages
- Verifica que `base` en `astro.config.mjs` coincida con el nombre de tu repositorio
- Asegúrate de que GitHub Pages esté configurado para usar GitHub Actions

### Las imágenes no se muestran
- Verifica que las rutas empiecen con `/` (e.g., `/images/author.jpg`)
- Confirma que los archivos estén en la carpeta `public/`

### Errores de build
```bash
# Limpiar y reinstalar
rm -rf node_modules .astro dist
npm install
npm run build
```

## Recursos Adicionales

- [Documentación de Astro](https://docs.astro.build)
- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [Markdown Guide](https://www.markdownguide.org/)

## Contacto

Si necesitas ayuda adicional, consulta la documentación oficial de Astro o abre un issue en el repositorio.
