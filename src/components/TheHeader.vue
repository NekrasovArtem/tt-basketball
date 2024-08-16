<script setup>
import { ref } from "vue";

const mobileMenu = ref(null);

// eslint-disable-next-line
function showMobileMenu() {
  console.log("bubuh");
  mobileMenu.value.classList.add("menu__active");
}

// eslint-disable-next-line
function hideMobileMenu() {
  console.log("blelele");
  mobileMenu.value.classList.remove("menu__active");
}
</script>

<template lang="pug">
header.header
  .mobile__menu(ref="mobileMenu")
    a.header__logo(href="https://www.xpage.ru/") 
      img(src="../assets/img/xpage.svg", alt="xpage")
    nav.mobile__menu__wrapper
      span.mobile__menu__item="Играть"
      span.mobile__menu__item="Смотреть"
      span.mobile__menu__item="Учиться"
      span.mobile__menu__item="Мероприятия"
    .menu__cross(@click="hideMobileMenu") 
      img.cross__img(src="../assets/img/menu__cross.svg", alt="Закрыть меню")
  .header__wrapper
    .header__navigation 
      a.header__logo(href="https://www.xpage.ru/") 
        img(src="../assets/img/xpage.svg", alt="xpage")
      nav.header__nav 
        a.nav__item(href="#")="Играть"
        a.nav__item(href="#")="Смотреть"
        a.nav__item(href="#")="Учиться"
        a.nav__item(href="#")="Мероприятия" 
    .header__menu.menu__mobile(@click="showMobileMenu") 
      .menu__wrapper
        span.menu__item
        span.menu__item
        span.menu__item
    a.header__logo.logo__mobile(href="https://www.xpage.ru/")
      img(src="../assets/img/xpage.svg", alt="xpage") 
    .header__user
      .header__menu.menu__desktop(@click="showMobileMenu") 
        .menu__wrapper
          span.menu__item
          span.menu__item
          span.menu__item
        span.menu__name="Меню"
      a.user__info(href="#")
        span.user__name="Геннадий П."
        img.user__image(src="../assets/img/user_photo.svg", alt="Аватарка") 
</template>
