<form action="{% url 'app_auth:logout' %}" method="post">
    {% csrf_token %}
    <button class="btn btn-primary mt-3" type="submit">Logout</button>
</form>
Це вирішення питання 405 помилки