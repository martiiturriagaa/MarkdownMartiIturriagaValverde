# Documentació del Bot de Discord

![Logotip de Discord](https://static0.howtogeekimages.com/wordpress/wp-content/uploads/2020/03/White-on-Blurple-Background-Discord.jpg)

Pots registrar la teva aplicació al [Portal de Desenvolupadors de Discord](https://discord.com/developers/applications).

Per fer que el bot respongui, escoltem l'esdeveniment `messageCreate` i utilitzem el mètode `message.reply()`.

```javascript
client.on('messageCreate', message => {
    if (message.content === 'ping') {
        message.reply('pong!');
    }
});