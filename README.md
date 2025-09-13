# Análisis de Seguridad y Hardening de un Servidor WordPress

**Proyecto final para la asignatura "Calidad, Seguridad y Auditoría Informática" del Máster Universitario en Ingeniería Informática.**

## Resumen del Proyecto

Este repositorio documenta un ejercicio completo de seguridad ofensiva y defensiva sobre una máquina virtual que aloja un servicio WordPress vulnerable. El proyecto abarca desde la explotación inicial y escalada de privilegios hasta el análisis forense post-incidente y la securización completa del sistema.

[**➡️ Descargar memoria en PDF(CSAI_Abastionado.pdf)**](CSAI_Abastionado.pdf)

---

## Fases del Proyecto

El trabajo se estructuró en cinco fases clave, cubriendo el ciclo de vida de un incidente de seguridad:

1.  [cite_start]**Pentesting y Obtención de Acceso:** Se identificaron y explotaron vulnerabilidades para obtener acceso inicial a la máquina[cite: 10]. [cite_start]Se utilizaron técnicas como inyección SQL para extraer credenciales de la base de datos y la explotación de un plugin para conseguir una reverse shell[cite: 59, 326, 327].
2.  [cite_start]**Análisis Forense Post-Explotación:** Tras comprometer la máquina, se realizó un análisis forense exhaustivo para reconstruir la cadena de ataque[cite: 707]. [cite_start]Se utilizaron herramientas como **Autopsy**, **GreenBone** y **Plaso** para analizar la imagen del sistema, identificar artefactos maliciosos y crear una cronología de los eventos[cite: 879, 999, 1135].
3.  [cite_start]**Securización del Sistema (Hardening):** Se implementó un plan de securización para remediar las vulnerabilidades encontradas[cite: 290]. [cite_start]Esto incluyó la limpieza de scripts maliciosos, la actualización de WordPress, el hardening de servicios como Apache, MariaDB y SSH, y la configuración de un firewall[cite: 1291, 1370, 1656, 1714].
4.  [cite_start]**Implementación de Auditoría:** Para asegurar la detección de futuros ataques, se configuraron herramientas de monitorización como **OSSEC** (HIDS) y **Fail2Ban** para proteger los servicios contra ataques de fuerza bruta[cite: 1912, 1930, 2021].
5.  [cite_start]**Propuestas de Mejora de Calidad:** Finalmente, se realizó un análisis de causa raíz y se propusieron mejoras en el ciclo de vida del software para prevenir incidentes similares en el futuro[cite: 2202].

---

## Tecnologías y Herramientas Utilizadas

* **Reconocimiento:** `Nmap`, `gobuster`, `WPScan`
* **Explotación:** `SQLmap`
* **Análisis Forense:** `Autopsy`, `GreenBone`, `Plaso`, `RKHunter`
* **Hardening y Auditoría:** `ufw`, `OSSEC`, `Fail2Ban`, `Logrotate`
* **Entorno:** Docker, WordPress, Apache, MariaDB, Linux

---

Este proyecto demuestra habilidades prácticas en pentesting, respuesta a incidentes, análisis forense y administración segura de sistemas.
