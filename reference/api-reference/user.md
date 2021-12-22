# User

## User GET-Requests

{% swagger method="get" path="/vX/user/:USERID" baseUrl="https://disweb.glitch.me" summary="Get information" %}
{% swagger-description %}
Get information about a discord user.
{% endswagger-description %}

{% swagger-parameter in="path" name="userid" type="snowflake" %}
The UserID of the respective (discord) user.
{% endswagger-parameter %}

{% swagger-response status="200: OK" description="" %}
Response example:

```javascript
{
    "username": "Wumpus#0000",
    "Bot": "True",
    "discriminator": "#0000",
    "avatar_url": "https://cdn.discordapp.com/avatars/814233207515643974/a_5fbd87e73c402c2ce62523578fedbb2f.gif?size=4096",
    "creation_date": "Wed Feb 24 2021 21:32:04 GMT+0100 (Mitteleuropäische Normalzeit)"
}
```
{% endswagger-response %}

{% swagger-response status="404: Not Found" description="" %}
```javascript
{
    // Response
}
```
{% endswagger-response %}
{% endswagger %}

