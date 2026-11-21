# Plan de trabajo · Grupo 03

| Integrante | Rol | Qué hace | Archivos o carpeta propios |
|---|---|---|---|
| Jhoan Mina | Coordinación y repositorio | Crea el repositorio público en GitHub y la carpeta plan/ con plan-de-trabajo.md y ficha-version.md. Redacta y mantiene el README.md con la descripción del proyecto, los integrantes y el enlace al sitio. Revisa que cada integrante haga sus 2 commits y que los mensajes sean claros. Coordina las fechas de los sprints y verifica que cada entrega se cumpla a tiempo. Junta las páginas del sitio web de cada integrante en un solo sitio. Entrega el enlace del repositorio en el campus virtual. | README.md, plan/ |
| David Campiño | Máquinas virtuales y red; seguridad y usuarios | Instala las dos máquinas virtuales con particionado manual y documenta cada paso. Configura la red entre las VMs y verifica la conectividad. Configura el acceso remoto por SSH y crea las instantáneas (snapshots) para poder volver a un estado estable. Crea los usuarios y el grupo proyecto, y asigna los permisos correspondientes. Configura el firewall para permitir solo el tráfico necesario. Guarda las capturas de pantalla de cada procedimiento como evidencia. | sprint-1.md, sprint-2.md, carpeta capturas-vm/ |
| Howard Lopez | Scripts y procesos; Docker; sitio web y videos | Escribe los dos scripts del proyecto, los prueba en las VMs y explica qué hacen. Crea el Dockerfile para contenerizar la aplicación y documenta cómo construir y ejecutar la imagen. Escribe el archivo YAML de Kubernetes para desplegar el contenedor. Elabora su parte del sitio web con la explicación de scripts, procesos y Docker. Graba los videos que muestran el funcionamiento y los entrega para el sitio. Registra su avance y evidencias en el archivo del sprint. | scripts/, docker/, sprint-3.md |

## Fechas de los sprints

| Sprint | Cierre (Yumbo) | Qué entregamos |
|---|---|---|
| 0 · Arranque | Viernes 20 de noviembre, 11:50 p. m. | Repositorio público con la carpeta plan y dentro sus respectivos archivos |
| 1 · Montaje | Viernes 27 de noviembre, 11:55 p. m. | Dos VMs, red, SSH e instantáneas |
| 2 · Servicios | Viernes 11 de diciembre, 11:55 p. m. | Usuarios, firewall, scripts, procesos y Docker |
| 3 · Cierre | Viernes 18 de diciembre, 11:55 p. m. | Imagen en Docker Hub, Kubernetes y sitio completo |

## Reglas del equipo

- **Flujo de trabajo en Git:** Cada integrante trabaja exclusivamente en sus archivos y carpetas asignadas para evitar conflictos de fusión (*merge conflicts*).
- **Commits claros:** Cada miembro debe realizar commits con nombres significativos por sprint con mensajes descriptivos (ej. `docs(sprint-1): agrega evidencias de red y SSH`).
- **Plazos internos:** Los avances y evidencias deben estar subidos al repositorio al menos **4 horas antes** del cierre oficial de cada sprint para dar margen a la revisión e integración final.
- **Comunicación:** Cualquier bloqueo técnico o retraso debe reportarse al grupo con anticipación para buscar apoyo sin comprometer la entrega.

## Repositorio

- **Enlace:** https://github.com/Jhoan09/proyecto-so-g03
