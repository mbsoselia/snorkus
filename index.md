---
layout: home
title: Блог выпускника Кембриджа
permalink: /
description: Это блог выпускника Кембриджа о том как поступить в английские школы и университеты из России.
---
<div class="jumbotron text-center">
    <h1>А вы готовы к учебе в Англии?</h1>
    <p>Узнайте зачем, как, куда и когда поступить.</p>
    <form class="form-inline" id="subscription-form">
        <div class="input-group">
            <input type="text" name="Ваш E-Mail" class="form-control white-border" size="50" placeholder="Ваш E-Mail">
            <div class="input-group-btn">
                <button type="submit" class="btn" id="postForm">Подписаться на Блог</button>
            </div>
        </div>
    </form>
</div>
<div id="modal-wrapper" class="modal">
    <div>
        <i class="fas fa-window-close modal-close"></i>
        <p>Спасибо за подписку!</p>
    </div>
</div>
<script>
    var $form = $('form#subscription-form'),
    url = 'https://script.google.com/macros/s/AKfycbxEyCidSvLTBOzT13G0om79Zuax88vU7s6ltYb4U9rOAs3W2lI/exec'

    $('#postForm').on('click', function(e) {
        e.preventDefault();
        var jqxhr = $.get(url, $form.serialize(), function(data) {
            console.log("Success! Data: " + data.statusText);
            // $(location).attr('href',redirectUrl);
            $('#modal-wrapper').toggleClass('show')
        });
    })

    $('.modal-close').on('click', function(f) {
        $('#modal-wrapper').removeClass("show")
    })
</script>