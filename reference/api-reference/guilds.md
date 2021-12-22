# Guilds

## Get guild informations

{% swagger baseUrl="https://disweb.glitch.me/v1" method="get" path="/guild/:GUILDID" summary="Get informations." %}
{% swagger-description %}
Get information about a discord server / guild.
{% endswagger-description %}

{% swagger-parameter in="path" type="snowflake" required="true" name="guildid" %}
The guild ID from the discord guild.
{% endswagger-parameter %}

{% swagger-response status="200" %}

{% endswagger-response %}

{% swagger-response status="401" description="Permission denied" %}

{% endswagger-response %}
{% endswagger %}



{% hint style="warning" %}
**IMPORTANT: You need the \[Disweb Discord Bot] for guild GET-requests**
{% endhint %}
