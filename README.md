[b][size=6]Qsdiscord - Integración Discord para tu servidor[/size][/b]

[b]Descripción:[/b]
Qsdiscord es un plugin de Minecraft que permite integrar tu servidor con un bot de Discord. 
Envía alertas, anuncios automáticos y sincroniza roles de Discord con tus jugadores de Minecraft. 
Además, permite vincular cuentas de jugadores con Discord y realizar acciones administrativas desde el juego.

[b]Características principales:[/b]
[list]
[*] Enviar mensajes a canales de Discord configurables.
[*] Vinculación de cuentas Minecraft ↔ Discord.
[*] Sincronización de roles en Discord automáticamente.
[*] Recarga de configuración, mensajes y alertas sin reiniciar el servidor.
[*] Pruebas de anuncios y alertas en tiempo real.
[*] Comandos administrativos para gestión avanzada.
[/list]

[b]Comandos:[/b]
[list]
[*][b]/qsdc reload [bot|config|alerts|messages|all][/b]  
    [i]Recarga parcial o total del plugin.[/i]  
    [u]Ejemplo:[/u] /qsdc reload bot → Reinicia solo el bot de Discord.

[*][b]/qsdc status[/b]  
    [i]Muestra si el bot de Discord está conectado.[/i]  
    [u]Ejemplo:[/u] /qsdc status → Bot conectado / desconectado.

[*][b]/qsdc alert [canal] [mensaje][/b]  
    [i]Envía un mensaje de alerta a un canal de Discord.[/i]  
    [u]Ejemplo:[/u] /qsdc alert general ¡El evento comienza en 10 minutos!

[*][b]/qsdc announce [canal] [mensaje][/b]  
    [i]Envía un anuncio a un canal de Discord.[/i]  
    [u]Ejemplo:[/u] /qsdc announce announcements ¡Servidor reiniciando en 5 minutos!

[*][b]/qsdc link[/b]  
    [i]Genera un código para vincular tu cuenta de Minecraft con Discord.[/i]  
    [u]Ejemplo:[/u] /qsdc link → Recibes un código para usar en Discord.

[*][b]/qsdc unlink[/b]  
    [i]Desvincula tu cuenta de Discord de tu jugador Minecraft.[/i]  
    [u]Ejemplo:[/u] /qsdc unlink → Se elimina la vinculación.

[*][b]/qsdc sync [jugador][/b]  
    [i]Sincroniza el rol de Discord de un jugador. Si no se indica jugador, se aplica al propio jugador.[/i]  
    [u]Ejemplo:[/u] /qsdc sync → Sincroniza tu rol.  
    [u]Ejemplo:[/u] /qsdc sync Steve → Sincroniza el rol de Steve.

[*][b]/qsdc setchannel <nombre> <id>[/b]  
    [i]Asigna un canal de Discord para alertas o anuncios.[/i]  
    [u]Ejemplo:[/u] /qsdc setchannel general 123456789012345678

[*][b]/qsdc resetcooldown [evento|jugador][/b]  
    [i]Resetea cooldowns de eventos o jugadores.[/i]  
    [u]Ejemplo:[/u] /qsdc resetcooldown → Resetea todos los cooldowns.  
    [u]Ejemplo:[/u] /qsdc resetcooldown Steve → Resetea los cooldowns de Steve.

[*][b]/qsdc announcetest <evento>[/b]  
    [i]Ejecuta un evento de prueba sin afectar el juego.[/i]  
    [u]Ejemplo:[/u] /qsdc announcetest monster_kill

[*][b]/qsdc adminlink <jugador> <discord_id>[/b]  
    [i]Vincula manualmente un jugador con un ID de Discord.[/i]  
    [u]Ejemplo:[/u] /qsdc adminlink Steve 123456789012345678

[*][b]/qsdc adminunlink <jugador>[/b]  
    [i]Desvincula un jugador de su Discord manualmente.[/i]  
    [u]Ejemplo:[/u] /qsdc adminunlink Steve
[/list]

[b]Permisos:[/b]
[list]
[*]qsdiscord.reload → Permite recargar configuraciones.
[*]qsdiscord.adminlink → Permite vincular cuentas manualmente.
[*]qsdiscord.adminunlink → Permite desvincular cuentas manualmente.
[*]qsdiscord.sync → Permite sincronizar roles de Discord.
[*]qsdiscord.alert → Permite enviar alertas.
[*]qsdiscord.announce → Permite enviar anuncios.
[*]qsdiscord.setchannel → Permite configurar canales.
[*]qsdiscord.announce.resetcooldown → Permite resetear cooldowns.
[*]qsdiscord.announce.test → Permite ejecutar eventos de prueba.
[/list]
