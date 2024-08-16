<script setup></script>

<template lang="pug">
header.header
  .header__wrapper
    .header__navigation 
      a.header__logo(href="https://www.xpage.ru/") 
        img(src="../assets/img/xpage.svg", alt="xpage")
      nav.header__nav 
        a.nav__item(href="#")="Играть"
        a.nav__item(href="#")="Смотреть"
        a.nav__item(href="#")="Учиться"
        a.nav__item(href="#")="Мероприятия" 
    .header__menu.menu__mobile 
      .menu__wrapper
        span.menu__item
        span.menu__item
        span.menu__item
    a.header__logo.logo__mobile(href="https://www.xpage.ru/")
      img(src="../assets/img/xpage.svg", alt="xpage") 
    .header__user
      .header__menu.menu__desktop 
        .menu__wrapper
          span.menu__item
          span.menu__item
          span.menu__item
        span.menu__name="Меню"
      a.user__info(href="#")
        span.user__name="Геннадий П."
        img.user__image(src="../assets/img/user_photo.svg", alt="Аватарка") 
</template>
