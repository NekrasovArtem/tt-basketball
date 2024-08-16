<script setup></script>

<template lang="pug">
section.section.section__learn 
  .section__head 
    h2.section__title="Учись"
    a.section__deep(href="#")
      span.deep__text="В раздел"
      img.deep__img(src="../assets/img/green_arrow.svg", alt="В раздел")
  .learn__wrapper
    .learn__main 
      .learn__sections 
        h3.learn__title="Мы собрали секции для детей по всему городу"
        .learn__tags 
          a.tag.tag__green="12 секций по всему городу"
      .learn__trainers
        h3.learn__title="Подбери тренера под свой уровень"
        .learn__tags 
          a.tag.tag__white="Детская тренировка"
          a.tag.tag__white="Для начинающих"
          a.tag.tag__white="Стритбол"
          a.tag.tag__white="Выезд тренера на дом"
          a.tag.tag__white="12 фильтров"
    .learn__side
      .learn__article 
        h3.article__title="Видеоуроки"
        .article__video
          .video__wrapper
            img.video__image(src="../assets/img/video_image.png", alt="")
          .article__wrapper 
            a.article__name(href="#")="Евгений Воронов: «Бронзовые медали - оценка труда нашей команды»"
            a.tag.tag__black(href="#")="26 октября"  
      hr.learn__line
      .learn__article
        h3.article__title="Статьи"
        .article__wrapper 
          a.article__name="Евгений Воронов: «Бронзовые медали - оценка труда нашей команды»"
          a.tag.tag__black(href="#")="26 октября" 
      hr.learn__line
      .learn__article
        h3.article__title="Термины"
        .learn__tags 
          a.tag.tag__black(href="#")="Треха"
          a.tag.tag__black(href="#")="Трехочковый бросок"
          a.tag.tag__black(href="#")="36 терминов" 

</template>
