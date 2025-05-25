# 📦 GLPI con Docker Compose

Este repositorio contiene una configuración lista para usar de **GLPI** utilizando **Docker Compose**. Ideal para pruebas, entornos de desarrollo o despliegues rápidos en servidores.

## 🧰 ¿Qué es GLPI?

[GLPI](https://glpi-project.org/) es una poderosa aplicación web de código abierto para la gestión de servicios de TI (ITSM), incluyendo inventario, helpdesk, gestión de activos, incidencias y más.

---

## 🚀 Cómo iniciar el entorno

### 1. Clona el repositorio

```bash
git clone https://github.com/tuusuario/glpi-docker.git
cd glpi-docker
````

### 2. Inicia los contenedores

```bash
docker-compose up -d
```

Esto levantará los servicios necesarios:

* `glpi`: servidor web con GLPI
* `mariadb`: base de datos para GLPI

---

## 🌐 Acceso a GLPI

Una vez que los contenedores estén arriba, accede desde tu navegador:

```
http://localhost:8080
```

(Si estás en un servidor, reemplaza `localhost` por la IP o dominio)

---

## 🔑 Credenciales por defecto

* **Usuario administrador:** `glpi`
* **Contraseña:** `glpi`

Otros usuarios disponibles (todos con contraseña `glpi`):

* **Técnico:** `tech`
* **Supervisor:** `super`
* **Usuario normal:** `normal`

> ⚠️ Se recomienda cambiar las contraseñas después de la instalación inicial.

---

## 🗃 Archivos importantes

* `docker-compose.yml` → Define los servicios y sus configuraciones.

---

## 🧽 Cómo detener y limpiar

```bash
docker-compose down
```

Si quieres borrar los volúmenes (datos):

```bash
docker-compose down -v
```

---

## ✅ Requisitos

* Docker
* Docker Compose

---

## 📌 Notas

* Esta configuración es para fines de desarrollo o entornos controlados.
* Para producción se recomienda asegurar la base de datos, usar HTTPS, y realizar backups regulares.

---

## ❤️ Agradecimientos

Proyecto GLPI: [https://github.com/glpi-project/glpi](https://github.com/glpi-project/glpi)
Documentación oficial: [https://glpi-user-documentation.readthedocs.io](https://glpi-user-documentation.readthedocs.io)

---

## ☕ ¿Te fue útil?

Si te sirvió este repositorio, puedes dejar una estrella ⭐ o invitarme un café: [PayPal](https://www.paypal.me/codadry)

