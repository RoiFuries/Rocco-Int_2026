<p align="center">
  <img src="assets/img/logo/logo.png" alt="Rocco Rodríguez" width="220">
</p>

<h1 align="center">Roccoweb</h1>
<p align="center"><em>Sitio portafolio de Rocco Rodríguez — Director de Fotografía, AMC</em></p>

<p align="center">
  <img src="https://img.shields.io/badge/estado-en%20desarrollo-EB5939" alt="estado: en desarrollo">
  <img src="https://img.shields.io/badge/stack-HTML%20%2F%20CSS%20%2F%20JS-1E1E1E" alt="stack">
  <img src="https://img.shields.io/badge/hosting-HostGator%20(FTP%20manual)-5D5D63" alt="hosting">
</p>

---

## Sobre el proyecto

Sitio portafolio para **Rocco Rodríguez**, director de fotografía (DP) y miembro de la AMC, con base en la Ciudad de México. Reúne trabajo comercial (Doritos, Volkswagen, Powerade, Bimbo, Amex, entre otros) y trabajo narrativo (series como *Monarca* y *El Rey*, además de proyectos de cine independiente), presentando cada proyecto con su video de Vimeo y notas técnicas de cámara y rodaje.

**Estado actual:** en desarrollo activo.

- ✅ **Fase 0** — navegación reconectada, un solo teléfono/correo en todo el sitio, limpieza de restos de la plantilla original (título incorrecto, oficinas falsas, carrito de compras, archivos duplicados).
- 🚧 **Fase 1** — pantalla de entrada dividida ("Narrative" / "Commercials") como nuevo home. Conviven por ahora dos versiones para comparar: `index.html` (fondo con fotografías) e `index2.html` (fondo con video de Vimeo).
- ⏳ **Fase 2** — contenido pendiente: premios reales, biografía, logos de clientes, un solo idioma, SEO.
- ⏳ **Fase 3** — pulido final, revisión de rendimiento y publicación.

## Estructura del proyecto

```
Roccoweb/
├── index.html              # Home (versión actual, fondo con fotos)
├── index2.html             # Home alterno (fondo con video de Vimeo) — en prueba
├── narrative_home.html     # Home del lado "Narrative" (aún sin diferenciar del template base)
├── commercial_home.html    # Home del lado "Commercials" (aún sin diferenciar del template base)
├── roco_about-me.html      # Página "About"
├── roco_portfolio.html     # Portafolio completo, con filtros por categoría
├── roco_contact.html       # Página de contacto
├── Projects/                # Una página de detalle por proyecto (video + ficha técnica)
├── assets/
│   ├── css/                 # Estilos (incluye main.css con la tipografía y colores base)
│   ├── js/                  # GSAP, Swiper, Slick, Isotope, etc.
│   ├── img/                  # Fotografía, logo, íconos
│   └── fonts/                 # Tipografías autohospedadas
├── temp/                    # Páginas de la plantilla original sin usar (referencia, no es parte del sitio en vivo)
└── _archivo_sin_usar/       # Archivos duplicados de la plantilla, retirados del sitio pero conservados
```

## Tecnología

HTML, CSS y JavaScript estático — sin build ni framework. Parte de una plantilla comercial de agencia creativa (Themepure) que se ha ido personalizando página por página con el contenido real de Rocco. Usa GSAP, Swiper, Slick e Isotope para animaciones, carruseles y los filtros del portafolio, y el reproductor de Vimeo para los videos embebidos de cada proyecto.

## Cómo verlo en local

Al ser HTML estático, basta con abrir cualquier archivo `.html` directo en el navegador. Para que las rutas y el JavaScript se comporten igual que en producción, es mejor levantar un servidor local sencillo:

```bash
cd Roccoweb
python3 -m http.server 8000
```

y abrir `http://localhost:8000` en el navegador.

## Contacto publicado en el sitio

- **Teléfono:** +52 55 3515 9210
- **Correo:** info@roccorodriguez.tv

*(Unificado en todas las páginas. Pendiente confirmar con Rocco si el teléfono se mantiene público por temas de privacidad.)*

## Despliegue

Publicación manual por FTP a HostGator. No hay integración automática (CI/CD): cada actualización se prueba en local y se sube a mano.

## Créditos

- **Desarrollo y personalización:** Rodrigo
- **Fotografía y dirección:** Rocco Rodríguez, AMC
- **Base de plantilla original:** Themepure
