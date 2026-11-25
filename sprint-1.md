# Sprint 1 · Montaje

[Volver al inicio](./)

- **Qué se pide en este sprint (5 puntos):** VM gráfica, VM de consola, red, SSH e instantáneas.
- **Qué se entrega en el campus:** el enlace de este sitio.
- **Qué más:** el video de 3 minutos (al final de esta página), 2 commits por integrante y el archivo `codigo_sprint1.txt` en el home del usuario principal de las dos VMs.

## 1. VM gráfica (g03-grafica)

Instalamos Fedora Workstation 45 con particionado manual: `/`, swap y `/home`. No usamos «borrar el disco». La VM tiene disco de 26,8 GB, 3 CPU y 8 GB de RAM.

| Partición | Tamaño | Por qué |
|---|---|---|
| / | 12 GB | Alberga Fedora Workstation 45, entorno gráfico y paquetes/herramientas instaladas con holgura. |
| swap | 2 GB | Apoya la memoria en picos de carga o suspensión sin gastar demasiado espacio del disco de 25 GB. |
| /home | 12,8 GB | Guarda archivos de usuario, configuraciones y repositorios/proyectos locales de forma separada. |


![Confirmación del método de instalación de Fedora Linux Workstation 45](capturas-vm/almacenamiento_final.png)  
*Figura 1: Se visualiza la confirmación del método de instalación de Fedora Linux Workstation 45, con el respectivo almacenamiento configurado.*

![Último paso de la instalación](capturas-vm/instalacion_final.png)  
*Figura 2: Se visualiza el último paso de la instalación.*

Comandos: `lsblk`, `df -h`, `cat /etc/fstab`, `date`

![Comando lsblk ejecutado en g03-grafica](capturas-vm/lsblk.png)  
*Figura 3: Se visualiza la terminal con el comando `lsblk` ejecutado.*

![Comando cat /etc/fstab ejecutado](capturas-vm/cat%20etcfstab.png)  
*Figura 4: Se visualiza la terminal con el comando `cat /etc/fstab` ejecutado.*

![Comando df -h ejecutado](capturas-vm/df%20-h.png)  
*Figura 5: Se visualiza la terminal con el comando `df -h` ejecutado.*

![Comando date ejecutado](capturas-vm/date.png)  
*Figura 6: Se visualiza la terminal con el comando `date` ejecutado.*

Dos navegadores y dos editores instalados:
| Navegador | Editor |
| :--- | :--- |
| Brave | Visual Studio |
| Chrome | Zed |

![Instalación de Brave Origin por terminal](capturas-vm/instalacion_braveorigin.png)  
*Figura 7: Se visualiza la instalación de Brave Origin mediante la terminal.*

![Continuación de la instalación de Brave Origin](capturas-vm/instalacion_braveorigin_2.png)  
*Figura 7.1: Se visualiza el resto del comando de instalación para Brave Origin.*

![Instalación de Google Chrome por terminal](capturas-vm/instalacion_chrome.png)  
*Figura 8: Se visualiza la instalación de Chrome por medio de la terminal.*

![Ambos navegadores abiertos en la VM](capturas-vm/navegadores%20abiertos.png)  
*Figura 9: Evidencia de ambos navegadores abiertos en la VM.*

## 2. VM de consola (g03-consola)

Instalamos Ubuntu Server 26.04 LTS con particionado manual: `/`, swap, `/home` y `/var`. Disco de 25 GB, 2 CPU y 2 GB de RAM (pasa a 3 GB en el Sprint 3, para Kubernetes).

| Partición | Tamaño | Por qué |
|---|---|---|
| / | [COMPLETAR] | [COMPLETAR: una frase] |
| /var | [COMPLETAR] | [COMPLETAR: una frase] |
| swap | [COMPLETAR] | [COMPLETAR: una frase] |
| /home | [COMPLETAR] | [COMPLETAR: una frase] |

Herramientas instaladas: make, rsync, curl, git y wget.

Comandos: `lsblk`, `df -h`, `cat /etc/fstab`, `sudo apt update`, `sudo apt install -y make rsync curl git wget`, `make --version`, `rsync --version`, `curl --version`, `git --version`, `wget --version`, `date`

![lsblk, df -h y cat /etc/fstab en g03-consola, con prompt y fecha](capturas-vm/s1-04-consola-lsblk.png)

[COMPLETAR: qué muestra la captura]

![Las cinco herramientas mostrando su versión](capturas-vm/s1-05-consola-herramientas.png)

[COMPLETAR: qué muestra la captura]

## 3. Red

Cada VM tiene dos adaptadores: el 1 en NAT (internet) y el 2 en red solo-anfitrión (para verse entre ellas). [COMPLETAR: qué direcciones tomó cada una y si hubo que configurar algo a mano]

Comandos: `ip a` en cada VM y `ping` en los dos sentidos.

![ip a en las dos VMs, mostrando una dirección en cada interfaz](capturas-vm/s1-06-ip-a.png)

[COMPLETAR: qué muestra la captura]

![ping de la gráfica a la consola y de la consola a la gráfica](capturas-vm/s1-07-ping.png)

[COMPLETAR: qué muestra la captura]

## 4. SSH

Entramos por SSH desde la VM gráfica a la VM de consola. [COMPLETAR: usuario y dirección usados]

Comando: `ssh usuario@direccion-de-la-consola`

![Sesión SSH abierta, con el prompt de la consola](capturas-vm/s1-08-ssh.png)

[COMPLETAR: qué muestra la captura]

## 5. Instantáneas

Una por VM, llamada `instalacion-limpia`, tomada con la VM apagada y la instalación terminada.

![Pestaña de instantáneas de g03-grafica](capturas-vm/s1-09-instantanea-grafica.png)

[COMPLETAR: qué muestra la captura]

![Pestaña de instantáneas de g03-consola](capturas-vm/s1-10-instantanea-consola.png)

[COMPLETAR: qué muestra la captura]

## Código del sprint

El docente publicó el código en el campus 48 horas antes del cierre. Lo guardamos en las dos VMs y lo mostramos en el video.

Comandos: `echo "CÓDIGO" > codigo_sprint1.txt`, `cat codigo_sprint1.txt` y `date`

## Video del sprint (3 minutos)

Pantalla continua y sin cortes. Cada integrante muestra su parte, dice su nombre y qué hizo en los primeros 10 segundos, y aparece su cara.

<iframe width="560" height="315" src="https://www.youtube.com/embed/ID_DEL_VIDEO" title="Sprint 1" frameborder="0" allowfullscreen></iframe>

## Lo que hizo cada integrante en este sprint

| Integrante | Qué hizo | Commits |
|---|---|---|
| Jhoan Mina | [COMPLETAR] | [COMPLETAR] |
| David Campiño | [COMPLETAR] | [COMPLETAR] |
| Howard López | [COMPLETAR] | [COMPLETAR] |

## Errores encontrados y fuentes consultadas

| Error | Causa probable | Solución | Fuente (título, enlace y fecha de consulta) |
|---|---|---|---|
| [COMPLETAR] | [COMPLETAR] | [COMPLETAR] | [COMPLETAR] |
