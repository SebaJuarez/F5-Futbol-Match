
<!-- PROJECT LOGO -->
<br />
<p align="center">
  <a href="https://github.com/pfrovdev/matchmaking-futbol-paw">
    <img src="https://github.com/user-attachments/assets/be273530-6750-46c1-965b-ee19e635c81e" alt="Matchmaking Fútbol 5">
  </a>
  <h3 align="center">Sistema de matchmaking para futbol amateur</h3>
  <p align="center"><a href="https://github.com/pfrovdev/matchmaking-futbol-paw"><strong>Explorar el repositorio</strong></a></p>
</p>


## Índice

* [Autores](#autores)
* [Acerca del Proyecto](#acerca-del-proyecto)
  * [Propósito](#propósito)
  * [Objetivos](#objetivos)
  * [Qué hace (resumen funcional)](#qué-hace-resumen-funcional)
* [Tecnologías Empleadas](#tecnologías-empleadas)
  * [Frontend](#frontend)
  * [Backend & Infraestructura](#backend-&-infraestructura)
  * [Base de datos y cache](#base-de-datos-y-cache)
  * [Otras herramientas](#otras-herramientas)
* [Cómo ejecutar en local](#cómo-ejecutar-en-local)

## Autores
* **Sebastián Juárez** - [SebaJuarez](https://github.com/SebaJuarez)
* **Agustín DePaola** - [Daggys](https://github.com/Dagyss)
* **Esteban Iarza**

## Acerca del Proyecto

### Propósito
**Matchmaking Fútbol 5** es una plataforma web diseñada para equipos de fútbol amateur que facilita la organización de partidos, optimiza el emparejamiento entre rivales equilibrados mediante un ranking ELO por equipos y fomenta la deportividad con un sistema de reputación.

### Objetivos
* Centralizar la organización de partidos y el historial de equipos.
* Mejorar la calidad de los emparejamientos utilizando un ranking ELO por equipos.
* Agilizar la coordinación entre capitanes y la confirmación de resultados.
* Proveer métricas básicas y reputación para incentivar el fair-play.

### Qué hace (resumen funcional)
* Creación y gestión de **equipos** (nombre, escudo, descripción, ubicación).
* Publicación y búsqueda de **desafíos** (partidos) por ranking y disponibilidad.
* Confirmación de resultados por ambas partes y registro de resultados.
* Cálculo y actualización automática del **ranking ELO** por equipo.
* Sistema de **reputación y calificación** post-partido.
* Historial de partidos y estadísticas básicas por equipo.
* Chat de coordinación: redirección a **WhatsApp** mediante enlace.

## Tecnologías Empleadas

### Frontend
(Interfaz server-rendered PHP + assets)

<a href="https://www.php.net/">
  <img src="https://img.shields.io/badge/PHP-777BB4?style=for-the-badge&logo=php&logoColor=white" alt="PHP" width=140>
</a>
<a href="https://developer.mozilla.org/en-US/docs/Web/HTML">
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5" width=120>
</a>
<a href="https://developer.mozilla.org/en-US/docs/Web/CSS">
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3" width=120>
</a>
<a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript">
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript" width=120>
</a>

**Descripción :** vistas renderizadas en servidor con PHP; assets en `public/` (CSS, JS, imágenes).

---

### Backend & Infraestructura

<a href="https://www.docker.com/">
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" alt="Docker" width=140>
</a>
<a href="https://kubernetes.io/">
  <img src="https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white" alt="Kubernetes" width=140>
</a>
<a href="https://www.terraform.io/">
  <img src="https://img.shields.io/badge/Terraform-7B42BC?style=for-the-badge&logo=terraform&logoColor=white" alt="Terraform" width=140>
</a>
<a href="https://jwt.io/">
  <img src="https://img.shields.io/badge/JWT-000000?style=for-the-badge" alt="JWT" width=120>
</a>
<a href="https://cloud.google.com/">
  <img src="https://img.shields.io/badge/GCP-4285F4?style=for-the-badge&logo=google-cloud&logoColor=white" alt="GCP" width=140>
</a>
<a href="https://www.gnu.org/software/make/">
  <img src="https://img.shields.io/badge/Make-000000?style=for-the-badge&logo=gnu&logoColor=white" alt="Make" width=120>
</a>
<a href="https://monologphp.github.io/">
  <img src="https://img.shields.io/badge/Monolog-2F3E46?style=for-the-badge" alt="Monolog" width=120>
</a>

**Descripción :** PHP en backend, JWT para auth, Docker + Kubernetes (GKE) para despliegue, Terraform para IaC. Makefile para comandos locales. Monolog para logging.

---

### Base de Datos y Cache

<a href="https://www.mysql.com/">
  <img src="https://img.shields.io/badge/MySQL-00758F?style=for-the-badge&logo=mysql&logoColor=white" alt="MySQL" width=140>
</a>
<a href="https://redis.io/">
  <img src="https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white" alt="Redis" width=140>
</a>

**Descripción :** MySQL como fuente de verdad (esquema relacional) y Redis para revocación y rotación de tokens.

---

### Otras herramientas

<a href="https://getcomposer.org/">
  <img src="https://img.shields.io/badge/Composer-7D8FAD?style=for-the-badge&logo=composer&logoColor=white" alt="Composer" width=140>
</a>
<a href="https://github.com/">
  <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" width=140>
</a>
<a href="https://github.com/filp/whoops">
  <img src="https://img.shields.io/badge/Whoops-error?style=for-the-badge&logo=php" alt="Whoops" width=120>
</a>
<a href="https://phpmailer.github.io/PHPMailer/">
  <img src="https://img.shields.io/badge/PHPMailer-Email?style=for-the-badge" alt="PHPMailer" width=120>
</a>
<a href="https://github.com/nrk/predis">
  <img src="https://img.shields.io/badge/Predis-RedisClient?style=for-the-badge" alt="Predis" width=120>
</a>

## Cómo ejecutar en local

**Requisitos:** Git, Docker, Make (opcional)

1. Clonar el repo:
```bash
git clone https://github.com/pfrovdev/matchmaking-futbol-paw.git
cd matchmaking-futbol-paw
```

2. Copiar el `.env.example` a `.env` y ajustar variables:
```bash
cp .env.example .env
# editar .env: DB credentials, JWT_SECRET, etc.
```

3. Levantar la pila:
```bash
make up
# o
docker compose up -d
```

4. Inicializar la base de datos:
```bash
make reset_db
# o ejecutar el SQL en src/Deploy_database/database_schema.sql
```

5. (Opcional) Cargar datos de demo:
```bash
make insertar_datos_demo
```

6. Acceder: `http://localhost:9999`

<!-- MARKDOWN LINKS -->
[contributors-shield]: https://img.shields.io/github/contributors/pfrovdev/matchmaking-futbol-paw.svg?style=flat-square
[contributors-url]: https://github.com/pfrovdev/matchmaking-futbol-paw/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/pfrovdev/matchmaking-futbol-paw.svg?style=flat-square
[forks-url]: https://github.com/pfrovdev/matchmaking-futbol-paw/network/members
[stars-shield]: https://img.shields.io/github/stars/pfrovdev/matchmaking-futbol-paw.svg?style=flat-square
[stars-url]: https://github.com/pfrovdev/matchmaking-futbol-paw/stargazers
[issues-shield]: https://img.shields.io/github/issues/pfrovdev/matchmaking-futbol-paw.svg?style=flat-square
[issues-url]: https://github.com/pfrovdev/matchmaking-futbol-paw/issues
