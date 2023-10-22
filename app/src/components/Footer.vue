<template>
    <div>
            <footer class="footer">
      <div class="footer__item footer__item1">
        <div class="footer__item_logo">
          <img src="../assets/img/Logo.svg" alt="" />
          <h1>Interno</h1>
        </div>
        <p class="footer__item_text">
          It is a long established fact that a reader will be distracted lookings.
        </p>
        <div class="footer__item_social">
          <img src="../assets/img/twitter.svg" alt="" /><a href="#"></a>

          <img src="../assets/img/in.svg" alt="" />
          <img src="" alt="" />
        </div>
      </div>
      <div class="footer__item2">
        <a class="footer__itme2_link" href="">Pages</a>
        <a class="footer__itme2_link" href="">Home</a>
        <a class="footer__itme2_link" href="">Project</a>
        <a class="footer__itme2_link" href="">Blog</a>
      </div>
      <div class="footer__item footer__item3">
        <h4 class="footer__item3_title">Contact</h4>
        <p class="footer__item3_text">
          55 East Birchwood Ave. <br />
          Brooklyn, New York 11201 <br />contact@interno.com (123) 456 - 7890
        </p>
      </div>
    </footer>
    </div>
</template>

<script>
    export default {
        
    }
</script>

<style lang="scss" scoped>
    .footer {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 60px;
  &__item {
    width: 393px;
    display: flex;
    flex-direction: column;
    gap: 10px;
    &_logo {
      display: flex;
      gap: 5px;
    }
    &_social {
      display: flex;
      gap: 30px;
    }
    &_text {
      font-family: Jost;
      font-size: 22px;
      font-weight: 400;
      line-height: 33px;
      letter-spacing: 0.01em;
      text-align: left;
    }
  }
  &__item2 {
    display: flex;
    flex-direction: column;
    gap: 10px;
    &_link {
      font-family: Jost;
      font-size: 22px;
      font-weight: 400;
      line-height: 66px;
      letter-spacing: 0.01em;
      text-align: left;
    }
  }
  &__item3 {
    &_title {
      font-family: DM Serif Display;
      font-size: 25px;
      font-weight: 400;
      line-height: 31px;
      letter-spacing: 0em;
      text-align: left;
    }
    &_text {
      font-family: Jost;
      font-size: 22px;
      font-weight: 400;
      line-height: 33px;
      letter-spacing: 0.01em;
      text-align: left;
    }
  }
}
</style>