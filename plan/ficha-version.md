# Ficha de verificación de versión · Grupo 03

Fecha de consulta: 17 de noviembre de 2026

## Fedora Workstation (VM gráfica: g03-grafica)

| Pregunta | Respuesta | Enlace |
|---|---|---|
| Versión y fecha | Fedora Workstation 45, lanzada el 3 de noviembre de 2026 | https://fedoramagazine.org/ |
| Actualizaciones de seguridad hasta | 24 de noviembre de 2027 (aprox. 13 meses por versión) | https://docs.fedoraproject.org/en-US/releases/lifecycle/ |
| Requisitos y VirtualBox | Mínimo 2 GB de RAM y 20 GB de disco; se recomienda el doble. Funciona en VirtualBox 7 como VM x86_64 | https://fedoraproject.org/workstation/download |
| Particionado manual | Sí: en el instalador web (Anaconda) con «Mount point assignment» o «Launch storage editor» en el menú ⋮ | https://anaconda-installer.readthedocs.io/en/latest/anaconda-webui/docs/installation-steps.html |
| Guía oficial de Docker Engine | Sí, para Fedora 43, 44 y 45 | https://docs.docker.com/engine/install/fedora/ |
| RAM asignada | 4 GB, porque GNOME pide más de 2 GB para andar fluido | — |

## Ubuntu Server (VM de consola: g03-consola)

| Pregunta | Respuesta | Enlace |
|---|---|---|
| Versión y fecha | Ubuntu Server 26.04 LTS «Resolute Raccoon» (punto 26.04.1), lanzada el 23 de abril de 2026 | https://documentation.ubuntu.com/release-notes/26.04/ |
| Actualizaciones de seguridad hasta | Abril de 2031 (soporte estándar); hasta 2036 con Ubuntu Pro | https://ubuntu.com/about/release-cycle |
| Requisitos y VirtualBox | Mínimo 1,5 GB de RAM y 4 GB de disco. Funciona en VirtualBox como VM x86_64 | https://documentation.ubuntu.com/release-notes/26.04/ |
| Particionado manual | Sí: opción «Custom storage layout» del instalador | https://documentation.ubuntu.com/server/ |
| Guía oficial de Docker Engine | Sí, Ubuntu 26.04 (LTS) está en la lista de versiones soportadas | https://docs.docker.com/engine/install/ubuntu/ |
| RAM asignada | 2 GB al instalar y 3 GB en el Sprint 3 para Kubernetes | — |

## Fedora (imagen base del Dockerfile)

| Pregunta | Respuesta | Enlace |
|---|---|---|
| Versión y fecha | fedora:45 (Fedora 45, 3 de noviembre de 2026) | https://hub.docker.com/_/fedora |
| Actualizaciones de seguridad hasta | 24 de noviembre de 2027, igual que Fedora 45 | https://docs.fedoraproject.org/en-US/releases/lifecycle/ |
| Requisitos | Imagen de unos 65 MB para linux/amd64; corre en cualquier host con Docker | https://hub.docker.com/_/fedora/tags |
| Particionado manual | No aplica: es una imagen de contenedor | — |
| Gestor de paquetes | dnf | https://docs.fedoraproject.org/ |
| Imagen en Docker Hub | Sí, imagen oficial con la etiqueta 45 | https://hub.docker.com/_/fedora/tags |
