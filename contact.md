---
layout: page
title: Связаться
subtitle: Есть вопросы? Пишите!
permalink: /связаться
description: Я надеюсь, что после того как вы прочитали мой блог, у вас остались вопрос на который я мог бы ответить лично. Если это так, то связаться со мной вы сможете тут.
---
<form class="container-fluid" id="contact-form" action="mailto:main@snorkusdomus.ru" method="POST" enctype="multipart/form-data" name="ContactForm">
    <div class="row">
        <div class="col-sm-6 form-group">
            <input title="namefield" class="form-control" id="name" name="name" placeholder="Имя" type="text" required>
        </div>
        <div class="col-sm-6 form-group">
            <input title="emailfield" class="form-control" id="email" name="email" placeholder="E-mail" type="email" required>
        </div>
    </div>
    <div class="row">
        <div class="col-sm-12 form-group"><textarea class="form-control" title="commentfield" id="comments" name="message" placeholder="Ваше сообщение" rows="5"></textarea><br></div>
    </div>
    <div class="row">
        <div class="col-sm-12 form-group">
            <button class="btn btn-coll center-block" title="submit-button" type="submit" id="postForm">Отправить</button>
        </div>
    </div>
</form>

<script type="text/javascript">
    var frmvalidator = new Validator(“ContactForm”); 
    frmvalidator.addValidation(“name”,”req”,”Пожалуйста, укажите ваше имя”);
    frmvalidator.addValidation(“email”,”req”,”Пожалуйста, укажите свой адрес электронной почты”); 
    frmvalidator.addValidation(“message”,”req”,”Пожалуйста, напишите ваше сообщение”); 
    frmvalidator.addValidation(“email”,”email”, “Пожалуйста, введите действительный адрес электронной почты”); 
</script>
