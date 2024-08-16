<script setup></script>

<template lang="pug">
footer.footer
  .footer__wrapper 
    .footer__content 
      .footer__info 
        .footer__head 
          h3.footer__title="Еще больше полезных материалов и видеоуроков в нашем приложении"
          .footer__stores
            a.store(href="#")
              img(src="../assets/img/app_store.svg", alt="Download on the App Store")
            a.store(href="#")
              img(src="../assets/img/google_play.svg", alt="Get it on Google Play")
        span.footer__copyright="Сделано в xpage"
      .footer__qrcode
        .qrcode
          img.qrcode__image(src="../assets/img/qrcode.svg", alt="QR-код")
          span.qrcode__os="iOS / Android"
          span.qrcode__text="Наведите камеру устройства на QR-код, чтобы скачать"
  img.footer__background(src="../assets/img/basketball_ball.png", alt="")
  img.footer__background.footer__background__mobile(src="../assets/img/basketball_ball_2.png", alt="")

</template>
