# Quick Start

## Make your first request

To make your first request, retrieve information about a Discord user.

{% swagger baseUrl="https://disweb.glitch.me" summary="Get information about a discord user" path="/vX/user/:USERID" method="get" %}
{% swagger-description %}
Get information about a discord user.

![Run in Postman](https://run.pstmn.io/button.svg)
{% endswagger-description %}

{% swagger-parameter in="body" name="userid" required="true" type="snowflake" %}
The (Discord) 

`userid`

 of the respective user.
{% endswagger-parameter %}

{% swagger-response status="200" description="Succesfully" %}
```javascript
{
    "name"="Wilson",
    "owner": {
        "id": "sha7891bikojbkreuy",
        "name": "Samuel Passet",
    "species": "Dog",}
    "breed": "Golden Retriever",
}
```
{% endswagger-response %}

{% swagger-response status="404: Not Found" description="Not found" %}

{% endswagger-response %}
{% endswagger %}
