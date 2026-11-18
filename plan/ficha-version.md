# Ficha de verificación de versión · Grupo 03

Fecha: 17 de noviembre de 2026 (enlaces consultados ese día)

## Fedora Workstation (VM gráfica: g03-grafica)

| Pregunta | Respuesta | Enlace |
|---|---|---|
| Versión y fecha | Fedora Workstation 45, lanzada el 3 de noviembre de 2026 | https://fedoraproject.org/workstation/ y https://docs.fedoraproject.org/en-US/releases/lifecycle/ |
| Actualizaciones de seguridad hasta | 24 de noviembre de 2027 (estimada: 4 semanas después del lanzamiento de Fedora 47; ≈13 meses por versión) | https://docs.fedoraproject.org/en-US/releases/lifecycle/ |
| Requisitos y VirtualBox | Mínimo oficial de unos 2 GB de RAM y 15–20 GB de disco; se recomiendan 4 GB de RAM y 20 GB o más. Funciona en VirtualBox 7.x como VM x86_64 con adaptador gráfico VMSVGA y 128 MB de vídeo. | https://docs.fedoraproject.org/en-US/fedora/latest/release-notes/welcome/Hardware_Overview/ |
| Particionado manual | Sí: en el instalador web (Anaconda) con «Mount point assignment» o «Launch storage editor» en el menú ⋮ | https://anaconda-installer.readthedocs.io/en/latest/anaconda-webui/docs/installation-steps.html |
| Guía oficial de Docker Engine | Sí, Fedora 43, 44 y 45 figuran como soportadas (comprobado el 17/11/2026) | https://docs.docker.com/engine/install/fedora/ |
| RAM asignada | 4 GB: es la cantidad recomendada para Fedora y la VM tiene entorno gráfico (GNOME). Decisión del grupo | https://docs.fedoraproject.org/en-US/fedora/latest/release-notes/welcome/Hardware_Overview/ |
| Firewall por defecto | firewalld, que viene instalado y activo. Se consulta con sudo firewall-cmd --state y sudo firewall-cmd --list-all. | https://docs.fedoraproject.org/en-US/quick-docs/firewalld/ |

## Ubuntu Server (VM de consola: g03-consola)

| Pregunta | Respuesta | Enlace |
|---|---|---|
| Versión y fecha | Ubuntu Server 26.04 LTS «Resolute Raccoon», lanzada el 23 de abril de 2026. El punto 26.04.1 se publicó en agosto de 2026 | https://documentation.ubuntu.com/release-notes/26.04/ |
| Actualizaciones de seguridad hasta | Abril de 2031 (soporte estándar de 5 años); hasta 2036 con Ubuntu Pro | https://ubuntu.com/about/release-cycle |
| Requisitos y VirtualBox | Mínimo 1,5 GB de RAM y 4 GB de disco, según las notas de la versión. Funciona en VirtualBox como VM x86_64 | https://documentation.ubuntu.com/release-notes/26.04/ |
| Particionado manual | Sí: opción «Custom storage layout» del instalador | https://documentation.ubuntu.com/server/ (buscar «storage» en la guía de instalación) |
| Guía oficial de Docker Engine | Sí, Ubuntu 26.04 (LTS) figura en la lista de versiones soportadas | https://docs.docker.com/engine/install/ubuntu/ |
| RAM asignada | 2 GB al instalar y 3 GB en el Sprint 3 para Kubernetes. Decisión del grupo, por encima del mínimo oficial de 1,5 GB | https://documentation.ubuntu.com/release-notes/26.04/ |
| Firewall por defecto | ufw viene instalado pero desactivado. Se activa con sudo ufw enable y se consulta con sudo ufw status verbose. | https://ubuntu.com/server/docs/how-to/security/firewalls/ |

## Fedora (imagen base del Dockerfile)

| Pregunta | Respuesta | Enlace |
|---|---|---|
| Versión y fecha | fedora:45 (Fedora 45, 3 de noviembre de 2026) | https://hub.docker.com/_/fedora |
| Actualizaciones de seguridad hasta | 24 de noviembre de 2027 (estimada, igual que Fedora 45) | https://docs.fedoraproject.org/en-US/releases/lifecycle/ |
| Requisitos | Imagen de unos 69 MB (aprox.; Docker Hub no desglosa el tamaño por arquitectura); linux/amd64 soportada; corre en cualquier host con Docker | https://hub.docker.com/_/fedora/tags |
| Particionado manual | No aplica: es una imagen de contenedor, no se instala en un disco | — |
| Gestor de paquetes | dnf (DNF5 en las versiones recientes de Fedora) | https://docs.fedoraproject.org/ |
| Imagen en Docker Hub | Sí, imagen oficial con la etiqueta `45` (también `latest`). Fedora la publica además en `registry.fedoraproject.org` | https://hub.docker.com/_/fedora/tags |
