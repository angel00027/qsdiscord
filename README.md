# QsDiscord - Integración avanzada de Discord para Minecraft

![QsDiscord](https://img.shields.io/badge/QsDiscord-Discord%20Integration-blue?style=flat-square)
![Version](https://img.shields.io/badge/version-1.0.0-green)
![Minecraft](https://img.shields.io/badge/Minecraft-1.20-blue)

---

## 📖 Descripción

QsDiscord es un plugin de Minecraft que conecta tu servidor directamente con Discord.
Con este complemento puedes:

* 📢 Enviar alertas y anuncios automáticos a canales de Discord.
* 🔧 Sincronizar roles de Discord con los rangos de tus jugadores.
* 🔗 Vincular cuentas de Minecraft con Discord para una experiencia integrada.
* 🛠 Ejecutar acciones administrativas desde el juego de forma segura y controlada.

---

## ⚙️ Compatibilidad / Softdepend

Este plugin funciona junto con varios complementos populares para maximizar su potencial:

* ✅ [PlaceholderAPI](https://www.spigotmc.org/resources/placeholderapi.6245/) → Para utilizar placeholders dinámicos en mensajes y alertas.
* ✅ [LuckPerms](https://www.spigotmc.org/resources/luckperms.28140/) → Para sincronizar rangos y roles entre Minecraft y Discord.
* ✅ [MythicMobs](https://www.spigotmc.org/resources/mythicmobs.5702/) → Permite enviar anuncios automáticos a Discord cuando un jefe aparece o es derrotado.

Estas dependencias aseguran que los eventos, roles y mensajes sean totalmente personalizables y sincronizados correctamente.

---

## 🌟 Características destacadas

* 📨 Envío de mensajes y alertas a canales de Discord configurables.
* 🔗 Vinculación de cuentas Minecraft ↔ Discord.
* 👑 Sincronización automática de roles según los rangos de los jugadores.
* 🔄 Recarga de configuración, mensajes y alertas sin reiniciar el servidor.
* 🧪 Pruebas de anuncios y alertas en tiempo real.
* 🛠 Comandos administrativos avanzados para gestión completa desde el juego.
* ⚡ Sistema de alertas configurable desde `alerts.yml` para personalizar cada notificación.

---

## 📂 Instalación

1. Descarga el archivo `.jar` del plugin.
2. Coloca el `.jar` en la carpeta `plugins` de tu servidor.
3. Asegúrate de tener instalados los softdepend necesarios: PlaceholderAPI, LuckPerms y MythicMobs (opcional según tus necesidades).
4. Reinicia tu servidor para generar los archivos de configuración.
5. Configura tu token de Discord y los canales en `config.yml`.

---

## 📝 Configuración

* `config.yml`: Configuración principal del bot de Discord, canales, roles y prefijos.
* `alerts.yml`: Configuración de alertas automáticas para comandos, eventos y placeholders.
* `announcements.yml`: Configuración de anuncios automáticos para eventos y placeholders.
* `messages.yml`: Personalización de mensajes, permisos y textos para comandos.

---

## 💻 Comandos principales

```
/qsdc reload [bot|config|alerts|messages|all] → Recarga parcial o total del plugin
/qsdc menu → Abre el menú de configuración
/qsdc status → Muestra si el bot de Discord está conectado
/qsdc alert [canal] [mensaje] → Envía un mensaje de alerta a Discord
/qsdc announce [canal] [mensaje] → Envía un anuncio a Discord
/qsdc link → Genera un código para vincular tu cuenta con Discord
/qsdc unlink → Desvincula tu cuenta de Discord
/qsdc sync [jugador] → Sincroniza roles de Discord
/qsdc setchannel <nombre> <id> → Configura canales de Discord
/qsdc resetcooldown [evento|jugador] → Restablece cooldowns
/qsdc announcetest <evento> → Prueba un evento sin afectar el juego
/qsdc adminlink <jugador> <discord_id> → Vincula un jugador manualmente
/qsdc adminunlink <jugador> → Desvincula un jugador manualmente
```

---

## 🔐 Permisos

* `qsdiscord.reload` → Recarga configuraciones del plugin.
* `qsdiscord.menu` → Abre el menú de configuración.
* `qsdiscord.adminlink` → Vincula cuentas manualmente.
* `qsdiscord.adminunlink` → Desvincula cuentas manualmente.
* `qsdiscord.sync` → Sincroniza roles de Discord.
* `qsdiscord.alert` → Envía alertas a Discord.
* `qsdiscord.announce` → Envía anuncios a Discord.
* `qsdiscord.setchannel` → Configura canales de Discord.
* `qsdiscord.announce.resetcooldown` → Reinicia tiempos de reutilización.
* `qsdiscord.announce.test` → Ejecuta eventos de prueba.

---

## 💬 Soporte y opinión

Si disfrutas del plugin o tienes sugerencias:

* ¿Tienes preguntas o problemas con el plugin?
  Únete a nuestro Discord para recibir ayuda rápida: [Haz clic aquí](https://discord.com/invite/KuyqQmgpx2)

* No olvides dejar tu calificación y comentario, ¡nos ayuda a mejorar el plugin continuamente! 😊

---

## 📄 Licencia

Este proyecto está bajo la [MIT License](LICENSE) – consulta el archivo LICENSE para más información.
