<form action="{% url 'app_auth:logout' %}" method="post">
    {% csrf_token %}
    <button class="btn btn-primary mt-3" type="submit">Logout</button>
</form>
Це вирішення питання 405 помилки



Vladyslav Babenko
  8:14 PM
Всім привіт, знайшов матеріал по питанню Віталя - з приводу Django MySql procedures
Джанго підтримує цей функціонал, ось документація
https://django-mssql.readthedocs.io/en/latest/usage.html#stored-procedures
В мене немає активної БД на MySQL - тому Віталій спробуй поюзати - і будемо чекати фідбек - чи це працює, зручно з цим працювати і т.д.
:+1:
1

New


Vladyslav Babenko
  9:03 PM
Друге питання було чому при виклику Author.objects - цей objects не підказував нам методи для роботи с БД
Відповідь тут: https://docs.djangoproject.com/en/5.0/topics/db/managers/
Почитайте по менеджери, мені допомогло явно вказати в моделі додаткове поле
objects = models.Manager()
Django ProjectDjango Project
Django
The web framework for perfectionists with deadlines.
