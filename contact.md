---
layout: page
title: Консультация
subtitle: Есть вопросы? Пишите!
permalink: /консультация
description: Я надеюсь, что после того как вы прочитали мой блог, у вас остались вопрос на который я мог бы ответить лично. Если это так, то связаться со мной вы сможете тут.
---
<form class="container-fluid" id="contact-form">
    <div class="row">
        <div class="col-sm-6 form-group">
            <input title="namefield" class="form-control" id="name" name="Имя" placeholder="Имя" type="text" required>
        </div>
        <div class="col-sm-6 form-group">
            <input title="emailfield" class="form-control" id="email" name="E-mail" placeholder="E-mail" type="email" required>
        </div>
    </div>
    <div class="row">
        <div class="col-sm-12 form-group"><input title="agefield" class="form-control" id="age" name="Сколько вам лет?" placeholder="Сколько вам лет?" rows="1" type="text" required></div>
    </div>
    <div class="row">
        <div class="col-sm-12 form-group"><input class="form-control" title="languagefield" id="english" name="Как вы изучаете английский?" placeholder="Как вы изучаете английский?" rows="1" type="text" required></div>
    </div>
    <div class="row">
        <div class="col-sm-12 form-group"><input class="form-control" title="schoolfield" id="school" name="Какая у вас успеваемость в школе?" placeholder="Какая у вас успеваемость в школе?" rows="1" type="text" required></div>
    </div>
    <div class="row">
        <div class="col-sm-12 form-group"><input class="form-control" title="englandfield" id="England" name="Насколько серьезно вы настроены на Англию?" placeholder="Насколько серьезно вы настроены на Англию?" rows="1" type="text" required></div>
    </div>
    <div class="row">
        <div class="col-sm-12 form-group"><input class="form-control" title="checkfield" id="confirm" name="Вы уже видели секцию 'Проверь Себя'?" placeholder="Вы уже видели секцию 'Проверь Себя'?" rows="1" type="text" required></div>
    </div>
    <div class="row">
        <div class="col-sm-12 form-group"><textarea class="form-control" title="commentfield" id="comments" name="Ваше сообщение" placeholder="Ваше сообщение" rows="5"></textarea><br></div>
    </div>
    <div class="row">
        <div class="col-sm-12 form-group">
            <button class="btn btn-coll center-block" title="submit-button" type="submit" id="postForm">Отправить</button>
        </div>
    </div>
</form>
<script type="text/javascript">
    var $form = $('form#contact-form'),
    url = 'https://script.google.com/macros/s/AKfycbx_65T093yhAYIIfPg4h91CCNWT8YknQgUIvRhkhdxdAot-BUI/exec',
        redirectUrl = 'cf-success-page.html'

    $('#postForm').on('click', function(e) {
      e.preventDefault();
      var jqxhr = $.get(url, $form.serialize(), function(data) {
                console.log("Success! Data: " + data.statusText);
          $(location).attr('href',redirectUrl);
            });
      })
</script>