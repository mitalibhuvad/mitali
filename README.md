# mitali
{% extends "base.html" %}
{% load static %}
{% block base_head %}
  <link rel="stylesheet" href="{% static 'css/signup.css' %}">
{% endblock %}

{% block content %}

<br/>
<br/>
<br/>
<br/>
<div class="form">
                <div class="note">
                    <p>Register to our website</p>
                </div>


                <div class="form-content">
                    <div class="row">
                        <div class="col-md-6">


                            <form method='post'>
                              {% csrf_token %}
                              {{ form.as_p }}
                              <button type="submit" class="btnSubmit">Sign up</button>
                            </form>
                          </div>
                    </div>
                </div>
</div>
<br/>
<br/>
{% endblock %}
