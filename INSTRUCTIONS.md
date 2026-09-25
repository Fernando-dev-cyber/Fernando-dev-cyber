# Guía Operativa del Portafolio

Guía práctica para el mantenimiento, despliegue y actualización continua de https://Fernando-dev-cyber.github.io.

---

## Tabla de Contenidos

1. [Estructura del Proyecto](#1-estructura-del-proyecto)
2. [Sincronización de CTFs (TryHackMe)](#2-sincronización-de-ctfs-tryhackme)
3. [Agregar Proyectos a la Portada](#3-agregar-proyectos-a-la-portada)
4. [Mantenimiento de SEO y Sitemap](#4-mantenimiento-de-seo-y-sitemap)
5. [Pruebas en Local](#5-pruebas-en-local)
6. [Publicación y CI/CD](#6-publicación-y-cicd)

---

## 1. Estructura del Proyecto

```text
/
├── index.html          Página principal (Hero, Sobre mí, Dominios, Skills, Proyectos, CTFs, Contacto)
├── 404.html            Página interactiva de error (Terminal Nmap)
├── sitemap.xml         Mapa del sitio indexable por motores de búsqueda
├── robots.txt          Directivas de rastreo para bots
│
├── css/
│   └── style.css       Hojas de estilo completas (variables de tema oscuro/claro, responsive)
│
├── js/
│   ├── main.js         Lógica interactiva (Matrix canvas, typewriter, switch de tema)
│   ├── ctf-data.js     Registro de salas de TryHackMe y configuraciones
│   └── blog-data.js    Estructura base para futuras publicaciones técnicas
│
├── scripts/
│   └── fetch-thm-rooms.mjs   Script Node.js que consulta la API de TryHackMe vía proxies
│
├── .github/workflows/
│   ├── static.yml      Pipeline de despliegue automático en GitHub Pages
│   └── thm-sync.yml    Workflow programado (cada 6h) para sincronizar salas de THM
│
└── INSTRUCTIONS.md     Esta guía operativa


---

### 👏 Créditos y Agradecimientos
* Diseño base e inspiración de arquitectura UI/UX por [Pranay Mokida](https://pranaymokida.xyz) ([@pranayesse](https://github.com/pranayesse)).
* Adaptado, traducido y reestructurado por Fernando Raúl Díaz Benites para análisis técnico y proyectos de Blue Team.

