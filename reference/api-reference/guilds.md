# Guilds

## Guild GET-Requests

{% swagger baseUrl="https://disweb.glitch.me/" method="get" path="vX/guild/:GUILDID" summary="Get informations." %}
{% swagger-description %}
Get information about a discord server / guild.
{% endswagger-description %}

{% swagger-parameter in="path" type="snowflake" required="true" name="guildid" %}
The guild ID from the discord guild.
{% endswagger-parameter %}

{% swagger-response status="200" description="Succesfully" %}
```
{
    "guildname": "Wumpusland",
    "guildID": "898212491409121280",
    "guildicon_url": "https://cdn.discordapp.com/icons/898212491409121280/ad0a24763d1fee5cde37784471e1dbd8.webp?size=4096",
    "guildroles_count": "36",
    "guildusers_count": "1,542",    
    "guildemojis_count": "14",
    "guildownerID": "866047167760039938",
    "guildcreation_date": "Thu Oct 14 2021 16:15:45 GMT+0200 (Mitteleuropäische Sommerzeit)",
    "creation_timestamp": 1614198724393
}
```
{% endswagger-response %}

{% swagger-response status="404: Not Found" description="Not found" %}
```javascript
{
    "Not found!"
}
```
{% endswagger-response %}
{% endswagger %}

{% hint style="warning" %}
**IMPORTANT: You need the** [**Disweb Discord Bot**](https://discord.com/oauth2/authorize?client\_id=922865205766135898\&permissions=274877959168\&scope=bot%20applications.commands) **for guild GET-requests**
{% endhint %}
