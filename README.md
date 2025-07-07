# 🚀 Leidi Portfolio - Portfolio Personal Moderno

Un portfolio personal desarrollado con **Astro**, diseñado para ser completamente estático, súper rápido y con un diseño moderno y responsivo. Perfecto para desarrolladores frontend que buscan mostrar sus habilidades y proyectos de manera profesional.

## 🌟 Características Principales

### ⚡ Rendimiento Excepcional
- **100% estático** - Sin JavaScript innecesario
- **Generado con Astro** - Carga ultra rápida
- **Optimizado para SEO** con meta tags completos
- **Responsive design** - Perfecto en todos los dispositivos
- **Tema oscuro/claro** automático según preferencias del usuario

### 🎨 Diseño Moderno
- **Componentes reutilizables** bien estructurados
- **Sistema de design tokens** con variables CSS
- **Iconos modernos** con Lucide Icons
- **Animaciones suaves** y efectos hover elegantes
- **Gradientes** y sombras profesionales
- **Tipografía** cuidadosamente seleccionada (Inter + JetBrains Mono)

### 📱 Totalmente Responsive
- **Mobile-first approach**
- **Breakpoints optimizados** (480px, 768px, 1024px)
- **Grid layouts** adaptativos
- **Imágenes optimizadas** con lazy loading

## 🛠️ Tecnologías Utilizadas

### Core
- **[Astro](https://astro.build/)** v5.11.0 - Framework principal
- **TypeScript** - Tipado estático
- **CSS Variables** - Sistema de design tokens
- **HTML semántico** - Accesibilidad mejorada

### Iconos y Assets
- **[Lucide Astro](https://lucide.dev/)** - Iconos SVG modernos
- **Google Fonts** - Inter & JetBrains Mono
- **Unsplash** - Imágenes de placeholder para proyectos

### Herramientas de Desarrollo
- **npm** - Gestión de paquetes
- **Astro Dev Server** - Desarrollo local con HMR
- **ESLint** (configuración futura)
- **Prettier** (configuración futura)

## 📁 Estructura del Proyecto

```
leidi-page/
├── public/                    # Assets estáticos
│   ├── favicon.svg           # Icono del sitio
│   └── og-image.jpg          # Imagen para Open Graph
├── src/
│   ├── components/           # Componentes reutilizables
│   │   ├── Header.astro      # Navegación principal
│   │   ├── Hero.astro        # Sección hero/inicio
│   │   ├── About.astro       # Sección sobre mí
│   │   ├── Projects.astro    # Showcase de proyectos
│   │   ├── Skills.astro      # Habilidades técnicas
│   │   ├── Contact.astro     # Información de contacto
│   │   └── Footer.astro      # Pie de página
│   ├── layouts/
│   │   └── Layout.astro      # Layout principal con meta tags
│   ├── pages/
│   │   └── index.astro       # Página principal
│   └── styles/
│       └── global.css        # Estilos globales y variables
├── astro.config.mjs          # Configuración de Astro
├── package.json              # Dependencias y scripts
├── tsconfig.json             # Configuración TypeScript
└── README.md                 # Documentación del proyecto
```

## 🚀 Instalación y Configuración

### Prerrequisitos
- **Node.js** v18.0.0 o superior
- **npm** v9.0.0 o superior

### Instalación

1. **Clona el repositorio**
   ```bash
   git clone https://github.com/tu-usuario/leidi-page.git
   cd leidi-page
   ```

2. **Instala las dependencias**
   ```bash
   npm install
   ```

3. **Inicia el servidor de desarrollo**
   ```bash
   npm run dev
   ```

4. **Abre tu navegador**
   ```
   http://localhost:4321
   ```

### Scripts Disponibles

```bash
# Desarrollo local con hot reload
npm run dev

# Construir para producción
npm run build

# Vista previa del build de producción
npm run preview

# Comandos de Astro
npm run astro
```

## 🎨 Personalización

### 1. **Colores y Branding**

Edita las variables CSS en `src/styles/global.css`:

```css
:root {
  /* Colores principales */
  --color-primary: #2563eb;        /* Azul principal */
  --color-primary-dark: #1d4ed8;   /* Azul oscuro */
  --color-secondary: #7c3aed;      /* Púrpura secundario */
  --color-accent: #f59e0b;         /* Amarillo acento */
  
  /* Personaliza según tu marca */
}
```

### 2. **Información Personal**

#### Header (`src/components/Header.astro`)
- Cambia el logo/nombre en la línea 15
- Modifica los enlaces de navegación

#### Hero (`src/components/Hero.astro`)
```astro
const heroData = {
  name: "Tu Nombre",
  title: "Tu Profesión",
  subtitle: "Tu descripción personalizada",
  // ...
};
```

#### About (`src/components/About.astro`)
```astro
const aboutData = {
  name: "Tu Nombre",
  location: "Tu Ciudad, País",
  experience: "X+ años",
  // Actualiza estadísticas e intereses
};
```

### 3. **Proyectos**

Edita `src/components/Projects.astro`:

```astro
const projects = [
  {
    title: "Tu Proyecto",
    description: "Descripción del proyecto",
    image: "URL_de_tu_imagen",
    technologies: [
      { name: "React", icon: Code2 },
      // Tus tecnologías
    ],
    liveUrl: "https://tu-proyecto.com",
    githubUrl: "https://github.com/tu-usuario/proyecto"
  }
];
```

### 4. **Habilidades**

Actualiza `src/components/Skills.astro`:

```astro
const skillCategories = [
  {
    title: "Frontend",
    skills: [
      { name: "React", level: 90 },
      // Tus habilidades con porcentajes
    ]
  }
];
```

### 5. **Información de Contacto**

Modifica `src/components/Contact.astro`:

```astro
const contactData = {
  email: "tu-email@dominio.com",
  phone: "+XX XXX XXX XXXX",
  location: "Tu Ciudad, País",
  // Actualiza todos los métodos de contacto
};
```

## 🎯 Secciones del Portfolio

### 1. **Header Navigation**
- Logo/nombre personalizable
- Navegación sticky con smooth scroll
- Responsive con menú hamburguesa (preparado para JS)

### 2. **Hero Section**
- Presentación personal impactante
- Call-to-action claros
- Elementos decorativos animados
- Placeholder para foto personal

### 3. **About Me**
- Historia personal y profesional
- Estadísticas de experiencia
- Intereses y pasiones
- Tarjeta de perfil elegante

### 4. **Projects Showcase**
- Grid responsive de proyectos
- Overlay con enlaces a demo y código
- Chips de tecnologías con iconos
- Imágenes optimizadas con lazy loading

### 5. **Skills & Technologies**
- Categorías organizadas (Frontend, Backend, etc.)
- Barras de progreso animadas
- Soft skills destacados
- Iconos representativos

### 6. **Contact Information**
- Múltiples métodos de contacto
- Enlaces directos (mailto, tel, WhatsApp)
- Información de disponibilidad
- Call-to-action final

### 7. **Footer**
- Enlaces a redes sociales
- Información adicional
- Créditos y tecnologías utilizadas

## 🌐 Despliegue

### Netlify (Recomendado)

1. **Conecta tu repositorio a Netlify**
2. **Configuración de build:**
   ```
   Build command: npm run build
   Publish directory: dist
   ```
3. **Deploy automático** en cada push

### Vercel

1. **Conecta tu repositorio a Vercel**
2. **Configuración automática** para Astro
3. **Deploy instantáneo**

### GitHub Pages

1. **Configura GitHub Actions**
2. **Build y deploy automático**
3. **Dominio personalizado** opcional

### Otros Servicios
- **Cloudflare Pages**
- **Surge.sh**
- **Firebase Hosting**

## 📊 Performance y SEO

### Optimizaciones Incluidas
- ✅ **Meta tags** completos (Open Graph, Twitter Cards)
- ✅ **Estructura semántica** HTML5
- ✅ **Lazy loading** de imágenes
- ✅ **Preconnect** a Google Fonts
- ✅ **Favicon** y manifest preparados
- ✅ **Sitemap** automático (Astro)
- ✅ **CSS minificado** en producción

### Métricas Esperadas
- **Performance:** 95+ (Lighthouse)
- **Accessibility:** 100 (Lighthouse)
- **Best Practices:** 100 (Lighthouse)
- **SEO:** 100 (Lighthouse)

## 🔧 Desarrollo y Contribución

### Estructura de Componentes

Cada componente sigue este patrón:

```astro
---
// 1. Imports de iconos y utilidades
import { Icon } from 'lucide-astro';

// 2. Datos estáticos del componente
const componentData = {
  // Configuración
};
---

<!-- 3. HTML del componente -->
<section class="component-section">
  <!-- Contenido -->
</section>

<style>
  /* 4. Estilos específicos del componente */
  .component-section {
    /* Estilos */
  }
  
  /* 5. Responsive */
  @media (max-width: 768px) {
    /* Móvil */
  }
  
  /* 6. Tema oscuro */
  @media (prefers-color-scheme: dark) {
    /* Dark mode */
  }
</style>
```

### Convenciones de CSS

- **Variables CSS** para consistencia
- **Mobile-first** approach
- **BEM-like** naming para clases
- **Transiciones** suaves en hover
- **Prefijos** de vendor automáticos

### Mejoras Futuras

- [ ] **Animaciones** con Intersection Observer
- [ ] **CMS** integration (Contenful/Strapi)
- [ ] **Blog** section con Markdown
- [ ] **Tema oscuro** toggle manual
- [ ] **Internacionalización** (i18n)
- [ ] **Analytics** integration
- [ ] **Formulario** de contacto con Netlify Forms

## 📝 Licencia

Este proyecto está bajo la Licencia MIT. Ver el archivo `LICENSE` para más detalles.

## 🤝 Contribuciones

Las contribuciones son bienvenidas. Por favor:

1. **Fork** el proyecto
2. **Crea** una rama para tu feature
3. **Commit** tus cambios
4. **Push** a la rama
5. **Abre** un Pull Request

## 📞 Contacto

**Leidi** - Desarrolladora Frontend

- 🌐 **Portfolio:** [tu-portfolio.com](https://tu-portfolio.com)
- 📧 **Email:** hola@leidi.dev
- 💼 **LinkedIn:** [linkedin.com/in/leidi](https://linkedin.com/in/leidi)
- 🐱 **GitHub:** [@leidi](https://github.com/leidi)

---

⭐ **¡Dale una estrella si te gustó el proyecto!** ⭐

Desarrollado con ❤️ usando **Astro** + **TypeScript** + **CSS moderno**

[![Open in StackBlitz](https://developer.stackblitz.com/img/open_in_stackblitz.svg)](https://stackblitz.com/github/withastro/astro/tree/latest/examples/minimal)
[![Open with CodeSandbox](https://assets.codesandbox.io/github/button-edit-lime.svg)](https://codesandbox.io/p/sandbox/github/withastro/astro/tree/latest/examples/minimal)
[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/withastro/astro?devcontainer_path=.devcontainer/minimal/devcontainer.json)

> 🧑‍🚀 **Seasoned astronaut?** Delete this file. Have fun!

## 🚀 Project Structure

Inside of your Astro project, you'll see the following folders and files:

```text
/
├── public/
├── src/
│   └── pages/
│       └── index.astro
└── package.json
```

Astro looks for `.astro` or `.md` files in the `src/pages/` directory. Each page is exposed as a route based on its file name.

There's nothing special about `src/components/`, but that's where we like to put any Astro/React/Vue/Svelte/Preact components.

Any static assets, like images, can be placed in the `public/` directory.

## 🧞 Commands

All commands are run from the root of the project, from a terminal:

| Command                   | Action                                           |
| :------------------------ | :----------------------------------------------- |
| `npm install`             | Installs dependencies                            |
| `npm run dev`             | Starts local dev server at `localhost:4321`      |
| `npm run build`           | Build your production site to `./dist/`          |
| `npm run preview`         | Preview your build locally, before deploying     |
| `npm run astro ...`       | Run CLI commands like `astro add`, `astro check` |
| `npm run astro -- --help` | Get help using the Astro CLI                     |

## 👀 Want to learn more?

Feel free to check [our documentation](https://docs.astro.build) or jump into our [Discord server](https://astro.build/chat).
