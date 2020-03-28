---
layout: page
title: А вы сможете поступить?
subtitle: Скачайте вступительные тесты и проверьте свои знания!
description: Проверьте свои знания и готовность к вступительным тестам в английских школах. А вы сможете поступить?
permalink: /проверь-себя
---
<div class="container-fluid cy text-center">
    <h3>Что я могу найти внизу?</h3>
    <p>Для каждего возраста внизу прилогаются полноценные вступительные тесты. Я призываю вас их <strong class="orange">распечатать и прорешать</strong>. Тем самым вы сможете понять на сколько они для вас трудные.</p>
<!--     <p>Если вам так же интересны <strong>выш уровень и области которые следует подтянуть</strong> (особенно во вступительных тестаз по английскому), то приглашаю вас воспользоваться моей услугой "<strong class="orange">Узнай Свой Результат!</strong>"</p> -->
</div>
<div class="container-fluid cy">
    <h3 class="text-center">Какие тесты мне подходят?</h3>
    <p>В <strong class="orange">Сентябре за год</strong> до начала учебы вам должно быть:</p>
    <ul>
        <li><strong>меньше 12и лет</strong> для поступления в Year 7 и следовательно <span class="orange">тестов 10+</span></li>
        <li><strong>меньше 14и лет</strong> для поступления в Year 9 и следовательно <span class="orange">тестов 12+</span></li>
        <li><strong>меньше 17и лет</strong> для поступления в Year 12 и следовательно <span class="orange">тестов 15+</span></li>
    </ul>
</div>
<div class="container-fluid">
    <button class="collapsible">Вступительные Тесты 10+</button>
    <div class="content">
        <a href="/assets/practice_papers/year-7-maths-specimen-paper-c.pdf" target="_blank"><div class="btn btn-coll wide-btn"><i class="fas fa-calculator icon-margin"></i>Математика</div></a>
        <a href="/assets/practice_papers/year-7-english-specimen-paper-c.pdf" target="_blank"><div class="btn btn-coll wide-btn"><i class="fas fa-book icon-margin"></i>английский</div></a>
<!--         <div class="btn btn-coll wide-btn"><i class="fas fa-check-double icon-margin"></i>Узнай Свой Результат!</div> -->
    </div>
    <button class="collapsible">Вступительные Тесты 12+</button>
    <div class="content">
        <a href="/assets/practice_papers/year-9-maths-specimen-paper-e.pdf" target="_blank"><div class="btn btn-coll wide-btn"><i class="fas fa-calculator icon-margin"></i>Математика</div></a>
        <a href="/assets/practice_papers/year-9-english-specimen-paper.pdf" target="_blank"><div class="btn btn-coll wide-btn"><i class="fas fa-book icon-margin"></i>английский</div></a>
<!--         <div class="btn btn-coll wide-btn"><i class="fas fa-check-double icon-margin"></i>Узнай Свой Результат!</div> -->
    </div>
    <button class="collapsible">Вступительные Тесты 15+</button>
    <div class="content">
        <a href="/assets/practice_papers/16-mathematics-specimen-examination.pdf" target="_blank"><div class="btn btn-coll wide-btn"><i class="fas fa-calculator icon-margin"></i>Математика</div></a>
        <a href="/assets/practice_papers/16-physics-specimen-examination.pdf" target="_blank"><div class="btn btn-coll wide-btn"><i class="fas fa-atom icon-margin"></i>Физика</div></a>
        <a href="/assets/practice_papers/16-chemistry-specimen-examination.pdf" target="_blank"><div class="btn btn-coll wide-btn"><i class="fas fa-vial icon-margin"></i>Химия</div></a>
        <a href="/assets/practice_papers/16-biology-specimen-examination.pdf" target="_blank"><div class="btn btn-coll wide-btn"><i class="fas fa-leaf icon-margin"></i>Биология</div></a>
        <a href="/assets/practice_papers/16-economics-specimen-examination.pdf" target="_blank"><div class="btn btn-coll wide-btn"><i class="fas fa-dollar-sign icon-margin"></i>Экономика</div></a>
<!--         <div class="btn btn-coll wide-btn"><i class="fas fa-check-double icon-margin"></i>Узнай Свой Результат!</div> -->
    </div>
</div>
<script>
    var coll = document.getElementsByClassName("collapsible");
    var i;

    for (i = 0; i < coll.length; i++) {
        coll[i].addEventListener("click", function() {
            this.classList.toggle("active");
            var content = this.nextElementSibling;
            if (content.style.display === "block") {
                content.style.display = "none";
            } else {
                content.style.display = "block";
            }
        });
    }
</script>