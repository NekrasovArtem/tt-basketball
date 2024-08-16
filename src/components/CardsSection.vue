<script setup>
// eslint-disable-next-line
const cardsInfo = [
  {
    title: "Найди себе команду",
    text: "Игры на районе - это возможность найти с кем поиграть в баскетбол в выходные, или создать свою игру и пригласить других игроков присоединиться.",
    button: "Найти",
    src: "./img/card_1.png",
  },
  {
    title: "Создавай команды",
    text: "Игры на районе - это возможность найти с кем поиграть в баскетбол в выходные, или создать свою игру и пригласить других игроков присоединиться.",
    button: "Создать",
    src: "./img/card_2.png",
  },
  {
    title: "Участвуй в турнирах",
    text: "Участвуйте в турнирах вместе с вашей командой. Будьте активными, побеждайте и получайте ачивки и призы от наших спонсоров.",
    button: "Участвовать",
    src: "./img/card_3.png",
  },
];
</script>

<template lang="pug">
section.section.section__cards 
  .section__head
    h2.section__title="Играй"
    a.section__deep(href="#")
      span.deep__text="В раздел"
      img.deep__img(src="../assets/img/orange_arrow.svg", alt="В раздел")
  .cards__wrapper 
    .card(v-for="card in cardsInfo")
      .card__wrapper 
        img.card__image(:src="card.src", :alt="card.title")
        .card__info 
          h3.card__title {{ card.title }}
          span.card__text {{ card.text }}
          button.card__button 
            span.button__text {{ card.button }}
            img.button__arrow(src="../assets/img/white_arrow.svg", alt="Подробнее")
</template>
