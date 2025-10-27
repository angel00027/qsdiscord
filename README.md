# QsDiscord

**QsDiscord** es un plugin de Minecraft que integra tu servidor con Discord, permitiendo enviar alertas, anuncios y sincronizar roles de jugadores con su cuenta de Discord. Compatible con **Spigot/Paper 1.20+**.

---

## 📜 Descripción

Con QsDiscord puedes:  

- Sincronizar roles de Discord con jugadores de Minecraft.  
- Enviar alertas y anuncios a canales de Discord configurables.  
- Vincular y desvincular cuentas de Discord de manera manual o automática.  
- Ejecutar eventos de prueba con placeholders y MythicMobs.  
- Resetear cooldowns de eventos por jugador o globalmente.  

El plugin es **compatible con**:  
- [PlaceholderAPI](https://www.spigotmc.org/resources/placeholderapi.6245/) (opcional, para placeholders)  
- [MythicMobs](https://www.spigotmc.org/resources/mythicmobs.5702/)  
- [LuckPerms](https://www.spigotmc.org/resources/luckperms.28140/) (opcional, para roles)  

---

## ⚙️ Instalación

1. Coloca el `.jar` de QsDiscord en la carpeta `plugins/` de tu servidor.  
2. Instala las dependencias necesarias: MythicMobs, PlaceholderAPI y LuckPerms (según funciones que uses).  
3. Reinicia tu servidor para que se generen los archivos de configuración.  
4. Configura los canales de Discord en `config.yml`.  

---

## 🛠 Comandos

| Comando | Descripción | Ejemplo |
|---------|------------|---------|
| `/qsdc reload <bot|config|alerts|messages|all>` | Recarga configuración o reinicia el bot de Discord. | `/qsdc reload bot` |
| `/qsdc adminlink <jugador> <discord_id>` | Vincula manualmente un jugador con un Discord ID. | `/qsdc adminlink Steve 123456789012345678` |
| `/qsdc adminunlink <jugador>` | Desvincula manualmente la cuenta de un jugador. | `/qsdc adminunlink Steve` |
| `/qsdc sync [jugador]` | Sincroniza roles de Discord de un jugador. Si no se indica jugador, sincroniza tu cuenta. | `/qsdc sync Alex` |
| `/qsdc resetcooldown [evento|jugador]` | Resetea cooldowns de eventos o jugadores. | `/qsdc resetcooldown bossfight` |
| `/qsdc announcetest <evento>` | Ejecuta un evento de prueba para ver cómo se enviaría a Discord. | `/qsdc announcetest welcome` |
| `/qsdc status` | Muestra si el bot de Discord está conectado. | `/qsdc status` |
| `/qsdc alert [canal] <mensaje>` | Envía un mensaje de alerta a Discord. | `/qsdc alert alerts ¡Servidor en mantenimiento!` |
| `/qsdc link` | Genera un código de vinculación para tu Discord (jugador). | `/qsdc link` |
| `/qsdc unlink` | Desvincula tu cuenta de Discord (jugador). | `/qsdc unlink` |
| `/qsdc announce [canal] <mensaje>` | Envía un anuncio a Discord. | `/qsdc announce announcements ¡Evento iniciado!` |
| `/qsdc setchannel <nombre> <id>` | Configura un canal de Discord para alertas o anuncios. | `/qsdc setchannel alerts 123456789012345678` |
| `/qsdc help` | Muestra la ayuda con todos los comandos disponibles. | `/qsdc help` |

---

## 🔑 Permisos

| Permiso | Descripción | Predeterminado |
|---------|------------|----------------|
| `qsdiscord.use` | Permite usar el comando principal `/qsdc`. | true |
| `qsdiscord.reload` | Permite recargar configuración y reiniciar el bot. | op |
| `qsdiscord.adminlink` | Permite vincular manualmente cuentas de Discord a jugadores. | op |
| `qsdiscord.adminunlink` | Permite desvincular manualmente cuentas de Discord de jugadores. | op |
| `qsdiscord.sync` | Permite sincronizar roles de Discord de jugadores. | op |
| `qsdiscord.alert` | Permite enviar alertas a Discord. | op |
| `qsdiscord.announce` | Permite enviar anuncios a Discord. | op |
| `qsdiscord.setchannel` | Permite configurar los canales de Discord. | op |
| `qsdiscord.announce.resetcooldown` | Permite resetear cooldowns de eventos o jugadores. | op |
| `qsdiscord.announce.test` | Permite ejecutar eventos de prueba en Discord. | op |

---

## 📂 Archivos de Configuración

- `config.yml` → Configuración principal del plugin y canales de Discord.  
- `messages.yml` → Mensajes personalizables para alertas, anuncios y comandos.  
- `alerts.yml` → Alertas automáticas configurables.  
- `announcements.yml` → Eventos y mensajes automáticos configurables.  

---

