<div align="center"><a name="readme-top"></a>


[![][image-banner]][vercel-link]

# LobeChat

Una interfaz/framework moderna y de código abierto para ChatGPT/LLMs con diseño elegante.<br/>
Soporta síntesis de voz, multimodal y sistema de plugins extensible (function calling).<br/>
Despliega tu aplicación privada de chat OpenAI ChatGPT/Claude/Gemini/Groq/Ollama con **UN CLIC GRATIS**.

**[English](./README.md)** · **Español** · [简体中文](./README.zh-CN.md) · [Sitio Oficial][official-site] · [Changelog][changelog] · [Documentación][docs] · [Blog][blog]

<!-- SHIELD GROUP -->

[![][github-release-shield]][github-release-link]
[![][docker-release-shield]][docker-release-link]
[![][vercel-shield]][vercel-link]
[![][discord-shield]][discord-link]<br/>
[![][github-contributors-shield]][github-contributors-link]
[![][github-forks-shield]][github-forks-link]
[![][github-stars-shield]][github-stars-link]
[![][github-issues-shield]][github-issues-link]
[![][github-license-shield]][github-license-link]

**Comparte el Repositorio LobeChat**

[![][share-x-shield]][share-x-link]
[![][share-telegram-shield]][share-telegram-link]
[![][share-whatsapp-shield]][share-whatsapp-link]
[![][share-reddit-shield]][share-reddit-link]
[![][share-linkedin-shield]][share-linkedin-link]

<sup>Pionero en la nueva era del pensamiento y la creación. Construido para ti, el Super Individuo.</sup>

![][image-overview]

</div>

## 🌟 ¿Qué es LobeChat?

**LobeChat** es una plataforma de chat con IA de código abierto que revoluciona la forma en que interactúas con los modelos de lenguaje. Diseñado con una interfaz moderna y elegante, LobeChat ofrece una experiencia de usuario excepcional mientras proporciona potentes capacidades de IA.

### ✨ Características Principales

🎯 **Interfaz Moderna y Elegante**
- Diseño cuidadosamente elaborado con soporte para temas claro y oscuro
- Interfaz responsive optimizada para dispositivos móviles y escritorio
- Aplicación Web Progresiva (PWA) para una experiencia nativa

🤖 **Soporte Multi-Modelo**
- Compatible con 40+ proveedores de IA incluyendo OpenAI, Claude, Gemini, Ollama
- Soporte para modelos locales y en la nube
- Capacidades multimodales: texto, imagen, voz y video

🔧 **Sistema de Plugins Avanzado**
- Más de 40 plugins disponibles para extender funcionalidades
- Soporte para Function Calling
- Integración con servicios externos y APIs

🎨 **Características Innovadoras**
- **Chain of Thought (CoT)**: Visualiza el proceso de razonamiento de la IA
- **Conversaciones Ramificadas**: Explora múltiples caminos de conversación
- **Artefactos**: Genera y visualiza contenido dinámico (SVG, HTML, documentos)
- **Base de Conocimiento**: Sube archivos y crea bases de conocimiento personalizadas

🗣️ **Capacidades de Voz**
- Texto a Voz (TTS) con múltiples voces de alta calidad
- Voz a Texto (STT) para conversaciones naturales
- Soporte para múltiples idiomas y acentos

🎨 **Generación de Imágenes**
- Integración con DALL-E 3, MidJourney, Pollinations
- Generación de imágenes desde texto
- Edición y manipulación de imágenes

## 🚀 Comenzar Rápidamente

### 🌐 Prueba Online

¡No necesitas instalación ni registro! Visita nuestro sitio web para experimentarlo de primera mano:

[![][vercel-shield-badge]][vercel-link]

### 🐳 Despliegue con Docker

La forma más rápida de ejecutar LobeChat en tu propio servidor:

```bash
# Crear directorio para almacenamiento
mkdir lobe-chat-db && cd lobe-chat-db

# Inicializar infraestructura de LobeChat
bash <(curl -fsSL https://lobe.li/setup.sh)

# Iniciar el servicio LobeChat
docker compose up -d
```

### ☁️ Despliegue en la Nube

Despliega LobeChat con un solo clic en tu plataforma favorita:

<div align="center">

| Vercel | Zeabur | Sealos | RepoCloud | Alibaba Cloud |
| :----: | :----: | :----: | :-------: | :-----------: |
| [![][deploy-button-image]][deploy-link] | [![][deploy-on-zeabur-button-image]][deploy-on-zeabur-link] | [![][deploy-on-sealos-button-image]][deploy-on-sealos-link] | [![][deploy-on-repocloud-button-image]][deploy-on-repocloud-link] | [![][deploy-on-alibaba-cloud-button-image]][deploy-on-alibaba-cloud-link] |

</div>

## 🎯 Casos de Uso

### 👨‍💼 Para Profesionales
- **Asistente de Productividad**: Automatiza tareas repetitivas y mejora la eficiencia
- **Análisis de Documentos**: Procesa y analiza documentos complejos
- **Generación de Contenido**: Crea contenido de marketing, blogs y documentación
- **Programación**: Asistencia en código, debugging y revisión de código

### 🎓 Para Educadores y Estudiantes
- **Tutor Personal**: Explicaciones personalizadas y ayuda con tareas
- **Investigación**: Búsqueda y síntesis de información académica
- **Aprendizaje de Idiomas**: Práctica conversacional y corrección gramatical
- **Preparación de Exámenes**: Generación de preguntas y material de estudio

### 🏢 Para Empresas
- **Atención al Cliente**: Chatbots inteligentes para soporte 24/7
- **Análisis de Datos**: Interpretación y visualización de datos empresariales
- **Capacitación**: Creación de material de entrenamiento personalizado
- **Automatización**: Integración con sistemas empresariales existentes

## 🛠️ Configuración Avanzada

### Variables de Entorno

Personaliza tu instalación con estas variables de entorno:

| Variable | Requerida | Descripción | Ejemplo |
|----------|-----------|-------------|---------|
| `OPENAI_API_KEY` | Sí | Tu clave API de OpenAI | `sk-xxxxxx...xxxxxx` |
| `OPENAI_PROXY_URL` | No | URL del proxy para OpenAI | `https://api.openai.com/v1` |
| `ACCESS_CODE` | No | Código de acceso para proteger tu servicio | `mi_codigo_secreto` |
| `OPENAI_MODEL_LIST` | No | Lista personalizada de modelos | `gpt-4,gpt-3.5-turbo` |

### 🔧 Desarrollo Local

Para desarrolladores que quieren contribuir o personalizar LobeChat:

```bash
# Clonar el repositorio
git clone https://github.com/seojcarlos/lobe-chat.git
cd lobe-chat

# Instalar dependencias
pnpm install

# Iniciar servidor de desarrollo
pnpm dev
```

## 🌍 Comunidad y Soporte

### 💬 Únete a Nuestra Comunidad

[![][discord-shield-badge]][discord-link]

Conecta con desarrolladores y usuarios entusiastas en nuestro Discord.

### 🤝 Contribuir

¡Las contribuciones son bienvenidas! Si estás interesado en contribuir:

1. 🍴 Haz fork del repositorio
2. 🔧 Crea una rama para tu feature (`git checkout -b feature/AmazingFeature`)
3. 💾 Commit tus cambios (`git commit -m 'Add some AmazingFeature'`)
4. 📤 Push a la rama (`git push origin feature/AmazingFeature`)
5. 🔄 Abre un Pull Request

### 📊 Estadísticas del Proyecto

<div align="center">

[![][github-contributors-shield]][github-contributors-link]
[![][github-forks-shield]][github-forks-link]
[![][github-stars-shield]][github-stars-link]

</div>

## 🏆 Reconocimientos

LobeChat ha sido reconocido por la comunidad de desarrolladores:

- ⭐ **Trending en GitHub**: Proyecto destacado en múltiples ocasiones
- 🌟 **Más de 50K estrellas**: Confianza de la comunidad global
- 🚀 **Adopción Empresarial**: Utilizado por empresas de todo el mundo
- 🎯 **Innovación**: Pionero en características como CoT y conversaciones ramificadas

## 📈 Rendimiento

LobeChat está optimizado para ofrecer el mejor rendimiento:

|                   Escritorio                   |                   Móvil                   |
| :--------------------------------------------: | :---------------------------------------: |
|              ![][chat-desktop]              |              ![][chat-mobile]              |
| [📑 Reporte Lighthouse][chat-desktop-report] | [📑 Reporte Lighthouse][chat-mobile-report] |

## 🔗 Ecosistema LobeHub

Descubre más productos del ecosistema LobeHub:

- **[🅰️ Lobe SD Theme][lobe-theme]**: Tema moderno para Stable Diffusion WebUI
- **[⛵️ Lobe Midjourney WebUI][lobe-midjourney-webui]**: Interfaz web para Midjourney
- **[🌏 Lobe i18n][lobe-i18n]**: Herramienta de automatización para traducción i18n
- **[💌 Lobe Commit][lobe-commit]**: Herramienta CLI para generar mensajes de commit

## 📄 Licencia

Este proyecto está licenciado bajo la Licencia Apache 2.0 - ver el archivo [LICENSE](./LICENSE) para más detalles.

---

<div align="center">

**¿Te gusta LobeChat? ¡Dale una ⭐ en GitHub!**

[![][image-star]][github-stars-link]

Hecho con ❤️ por [seojcarlos](https://github.com/seojcarlos)

</div>

<!-- ENLACES -->
[back-to-top]: https://img.shields.io/badge/-VOLVER_ARRIBA-151515?style=flat-square
[blog]: https://lobehub.com/blog
[changelog]: https://lobehub.com/changelog
[chat-desktop]: https://raw.githubusercontent.com/lobehub/lobe-chat/lighthouse/lighthouse/chat/desktop/pagespeed.svg
[chat-desktop-report]: https://lobehub.github.io/lobe-chat/lighthouse/chat/desktop/chat_preview_lobehub_com_chat.html
[chat-mobile]: https://raw.githubusercontent.com/lobehub/lobe-chat/lighthouse/lighthouse/chat/mobile/pagespeed.svg
[chat-mobile-report]: https://lobehub.github.io/lobe-chat/lighthouse/chat/mobile/chat_preview_lobehub_com_chat.html
[deploy-button-image]: https://vercel.com/button
[deploy-link]: https://vercel.com/new/clone?repository-url=https%3A%2F%2Fgithub.com%2Fseojcarlos%2Flobe-chat&env=OPENAI_API_KEY,ACCESS_CODE&envDescription=Encuentra%20tu%20clave%20API%20de%20OpenAI%20haciendo%20clic%20en%20el%20botón%20Aprende%20Más.%20%7C%20El%20Código%20de%20Acceso%20puede%20proteger%20tu%20sitio%20web&envLink=https%3A%2F%2Fplatform.openai.com%2Faccount%2Fapi-keys&project-name=lobe-chat&repository-name=lobe-chat
[deploy-on-alibaba-cloud-button-image]: https://service-info-public.oss-cn-hangzhou.aliyuncs.com/computenest-en.svg
[deploy-on-alibaba-cloud-link]: https://computenest.console.aliyun.com/service/instance/create/default?type=user&ServiceName=LobeChat%E7%A4%BE%E5%8C%BA%E7%89%88
[deploy-on-repocloud-button-image]: https://d16t0pc4846x52.cloudfront.net/deploylobe.svg
[deploy-on-repocloud-link]: https://repocloud.io/details/?app_id=248
[deploy-on-sealos-button-image]: https://raw.githubusercontent.com/labring-actions/templates/main/Deploy-on-Sealos.svg
[deploy-on-sealos-link]: https://template.usw.sealos.io/deploy?templateName=lobe-chat-db
[deploy-on-zeabur-button-image]: https://zeabur.com/button.svg
[deploy-on-zeabur-link]: https://zeabur.com/templates/VZGGTI
[discord-link]: https://discord.gg/AYFPHvv2jT
[discord-shield]: https://img.shields.io/discord/1127171173982154893?color=5865F2&label=discord&labelColor=black&logo=discord&logoColor=white&style=flat-square
[discord-shield-badge]: https://img.shields.io/discord/1127171173982154893?color=5865F2&label=discord&labelColor=black&logo=discord&logoColor=white&style=for-the-badge
[docker-release-link]: https://hub.docker.com/r/lobehub/lobe-chat-database
[docker-release-shield]: https://img.shields.io/docker/v/lobehub/lobe-chat-database?color=369eff&label=docker&labelColor=black&logo=docker&logoColor=white&style=flat-square&sort=semver
[docs]: https://lobehub.com/docs/usage/start
[github-contributors-link]: https://github.com/seojcarlos/lobe-chat/graphs/contributors
[github-contributors-shield]: https://img.shields.io/github/contributors/seojcarlos/lobe-chat?color=c4f042&labelColor=black&style=flat-square
[github-forks-link]: https://github.com/seojcarlos/lobe-chat/network/members
[github-forks-shield]: https://img.shields.io/github/forks/seojcarlos/lobe-chat?color=8ae8ff&labelColor=black&style=flat-square
[github-issues-link]: https://github.com/seojcarlos/lobe-chat/issues
[github-issues-shield]: https://img.shields.io/github/issues/seojcarlos/lobe-chat?color=ff80eb&labelColor=black&style=flat-square
[github-license-link]: https://github.com/seojcarlos/lobe-chat/blob/main/LICENSE
[github-license-shield]: https://img.shields.io/badge/license-apache%202.0-white?labelColor=black&style=flat-square
[github-release-link]: https://github.com/seojcarlos/lobe-chat/releases
[github-release-shield]: https://img.shields.io/github/v/release/seojcarlos/lobe-chat?color=369eff&labelColor=black&logo=github&style=flat-square
[github-stars-link]: https://github.com/seojcarlos/lobe-chat/network/stargazers
[github-stars-shield]: https://img.shields.io/github/stars/seojcarlos/lobe-chat?color=ffcb47&labelColor=black&style=flat-square
[image-banner]: https://github.com/user-attachments/assets/6f293c7f-47b4-47eb-9202-fe68a942d35b
[image-overview]: https://github.com/user-attachments/assets/dbfaa84a-2c82-4dd9-815c-5be616f264a4
[image-star]: https://github.com/user-attachments/assets/c3b482e7-cef5-4e94-bef9-226900ecfaab
[lobe-commit]: https://github.com/lobehub/lobe-commit/tree/master/packages/lobe-commit
[lobe-i18n]: https://github.com/lobehub/lobe-commit/tree/master/packages/lobe-i18n
[lobe-midjourney-webui]: https://github.com/lobehub/lobe-midjourney-webui
[lobe-theme]: https://github.com/lobehub/sd-webui-lobe-theme
[official-site]: https://lobehub.com
[share-linkedin-link]: https://linkedin.com/feed
[share-linkedin-shield]: https://img.shields.io/badge/-compartir%20en%20linkedin-black?labelColor=black&logo=linkedin&logoColor=white&style=flat-square
[share-reddit-link]: https://www.reddit.com/submit?title=Mira%20este%20repositorio%20de%20GitHub%20%F0%9F%A4%AF%20LobeChat%20-%20Una%20interfaz%20de%20código%20abierto%2C%20extensible%20y%20de%20alto%20rendimiento%20para%20chatbots.%20Soporta%20despliegue%20gratuito%20con%20un%20clic%20de%20tu%20aplicación%20web%20ChatGPT%2FLLM%20privada.%20%23chatbot%20%23chatGPT%20%23openAI&url=https%3A%2F%2Fgithub.com%2Fseojcarlos%2Flobe-chat
[share-reddit-shield]: https://img.shields.io/badge/-compartir%20en%20reddit-black?labelColor=black&logo=reddit&logoColor=white&style=flat-square
[share-telegram-link]: https://t.me/share/url"?text=Mira%20este%20repositorio%20de%20GitHub%20%F0%9F%A4%AF%20LobeChat%20-%20Una%20interfaz%20de%20código%20abierto%2C%20extensible%20y%20de%20alto%20rendimiento%20para%20chatbots.%20Soporta%20despliegue%20gratuito%20con%20un%20clic%20de%20tu%20aplicación%20web%20ChatGPT%2FLLM%20privada.%20%23chatbot%20%23chatGPT%20%23openAI&url=https%3A%2F%2Fgithub.com%2Fseojcarlos%2Flobe-chat
[share-telegram-shield]: https://img.shields.io/badge/-compartir%20en%20telegram-black?labelColor=black&logo=telegram&logoColor=white&style=flat-square
[share-whatsapp-link]: https://api.whatsapp.com/send?text=Mira%20este%20repositorio%20de%20GitHub%20%F0%9F%A4%AF%20LobeChat%20-%20Una%20interfaz%20de%20código%20abierto%2C%20extensible%20y%20de%20alto%20rendimiento%20para%20chatbots.%20Soporta%20despliegue%20gratuito%20con%20un%20clic%20de%20tu%20aplicación%20web%20ChatGPT%2FLLM%20privada.%20https%3A%2F%2Fgithub.com%2Fseojcarlos%2Flobe-chat%20%23chatbot%20%23chatGPT%20%23openAI
[share-whatsapp-shield]: https://img.shields.io/badge/-compartir%20en%20whatsapp-black?labelColor=black&logo=whatsapp&logoColor=white&style=flat-square
[share-x-link]: https://x.com/intent/tweet?hashtags=chatbot%2CchatGPT%2CopenAI&text=Mira%20este%20repositorio%20de%20GitHub%20%F0%9F%A4%AF%20LobeChat%20-%20Una%20interfaz%20de%20código%20abierto%2C%20extensible%20y%20de%20alto%20rendimiento%20para%20chatbots.%20Soporta%20despliegue%20gratuito%20con%20un%20clic%20de%20tu%20aplicación%20web%20ChatGPT%2FLLM%20privada.&url=https%3A%2F%2Fgithub.com%2Fseojcarlos%2Flobe-chat
[share-x-shield]: https://img.shields.io/badge/-compartir%20en%20x-black?labelColor=black&logo=x&logoColor=white&style=flat-square
[vercel-link]: https://chat-preview.lobehub.com
[vercel-shield]: https://img.shields.io/badge/vercel-online-55b467?labelColor=black&logo=vercel&style=flat-square
[vercel-shield-badge]: https://img.shields.io/badge/PRUEBA%20LOBECHAT-ONLINE-55b467?labelColor=black&logo=vercel&style=for-the-badge
