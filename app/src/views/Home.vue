
<script>
import Header from '@/components/Header.vue';



export default {
  name: "App",
  components: {
    Header
},
   
};
</script>

<template>

  <div id="app">
    
    <div class="top_top">
      <section class="top">
        <h1 class="top__title">
          Let Your Home <br />
          Be Unique
        </h1>
        <p class="top__text">
          There are many variations of <br />
          the passages of lorem Ipsum fromavailable, majority.
        </p>
        <button class="top__button">
          <a href=""><span class="top__button_text">Get started</span></a
          ><img src="../assets/img/Vector@2x.svg" alt="" />
        </button>
      </section>
    </div>
    <section class="projects">
      <div class="projects__heading">
        <h1 class="projects__heading_title">Follow Our Projects</h1>
        <p class="projects__heading_text">
          It is a long established fact that a reader will be distracted by the of
          readable content of page lookings at its layouts points.
        </p>
      </div>
      <div class="projects__catalog">
        <div class="projects__catalog_box">
          <div class="projects__item">
            <img src="../assets/img/product1.png" alt="" class="projects__item_img" />
            <div class="projects__item_description">
              <h3 class="projects__item_title">Modern Kitchan</h3>
              <p class="projects__item_text">Decor / Artchitecture</p>
              <img src="../assets/img/strelka.svg" alt="" class="projects__iten_strelka" />
            </div>
          </div>
          <div class="projects__item">
            <img src="../assets/img/product2.png" alt="" class="projects__item_img" />
            <div class="projects__item_description">
              <h3 class="projects__item_title">Modern Kitchan</h3>
              <p class="projects__item_text">Decor / Artchitecture</p>
              <img src="../assets/img/strelka.svg" alt="" class="projects__iten_strelka" />
            </div>
          </div>
          <div class="projects__item">
            <img src="../assets/img/product3.png" alt="" class="projects__item_img" />
            <div class="projects__item_description">
              <h3 class="projects__item_title">Modern Kitchan</h3>
              <p class="projects__item_text">Decor / Artchitecture</p>
              <img src="../assets/img/strelka.svg" alt="" class="projects__iten_strelka" />
            </div>
          </div>
          <div class="projects__item">
            <img src="../assets/img/product4.png" alt="" class="projects__item_img" />
            <div class="projects__item_description">
              <h3 class="projects__item_title">Modern Kitchan</h3>
              <p class="projects__item_text">Decor / Artchitecture</p>
              <img src="../assets/img/strelka.svg" alt="" class="projects__iten_strelka" />
            </div>
          </div>
        </div>
      </div>
    </section>
    <section class="middle">
      <div class="middle__item">
        <h1 class="middle__item_title">12</h1>
        <p class="middle__item_p">Years Of Experiance</p>
      </div>
      <div class="middle__item">
        <h1 class="middle__item_title">85</h1>
        <p class="middle__item_p">Success Project</p>
      </div>
      <div class="middle__item">
        <h1 class="middle__item_title">15</h1>
        <p class="middle__item_p">Active Project</p>
      </div>
      <div class="middle__item">
        <h1 class="middle__item_title">95</h1>
        <p class="middle__item_p">Happy CUstomers</p>
      </div>
    </section>
    <section class="down">
      <div class="down__heading">
        <h1 class="down__heading_title">Articles & News</h1>
        <p class="down__heading_text">
          It is a long established fact that a reader will be distracted by the of
          readable content <br />
          of a page when lookings at its layouts the points of using.
        </p>
      </div>
      <div class="down__items">
        <div class="down__item">
          <img class="down__item_img" src="../assets/img/down1.png" alt="" />
          <h3 class="down__item_title">
            Let’s Get Solution For Building Construction Work
          </h3>
          <p class="down__item_text">26 December,2022</p>
          <img src="../assets/img/strelka.svg" alt="" />
        </div>
        <div class="down__item">
          <img class="down__item_img" src="../assets/img/down2.png" alt="" />
          <h3 class="down__item_title">
            Let’s Get Solution For Building Construction Work
          </h3>
          <p class="down__item_text">26 December,2022</p>
          <img src="../assets/img/strelka.svg" alt="" />
        </div>
        <div class="down__item">
          <img class="down__item_img" src="../assets/img/down3.png" alt="" />
          <h3 class="down__item_title">
            Let’s Get Solution For Building Construction Work
          </h3>
          <p class="down__item_text">26 December,2022</p>
          <img src="../assets/img/strelka.svg" alt="" />
        </div>
      </div>
    </section>

  </div>
</template>

<style lang="scss">


* {
  margin: 0;
  padding: 0;
  text-decoration: none;
}
.center {
  padding-left: calc(50% - 100% / 2);
  padding-right: calc(50% - 100% / 2);
}
a {
  color: black;
}
.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  &__item {
    display: flex;
    align-items: center;
  }
  &__item1 {
    gap: 3px;
    padding-left: 300px;
  }
  &__item2 {
    gap: 30px;
    padding-right: 300px;
  }
}
.top {
  &_top {
    display: flex;
    justify-content: center;
  }
  display: flex;
  border-radius: 7% 0% 0% 7%;
  flex-direction: column;
  justify-content: center;
  flex-wrap: nowrap;
  align-content: center;
  width: 1201px;
  height: 758px;
  align-items: start;
  padding-left: 100px;
  &__button {
    background-color: #292f36;
    display: flex;
    gap: 5px;
    width: 220px;
    height: 75px;
    border-radius: 10%;
    justify-content: center;
    align-items: center;
    &_text {
      font-family: Jost;
      font-size: 18px;
      font-weight: 600;
      line-height: 23px;
      letter-spacing: 0.02em;
      text-align: center;
      color: white;
    }
  }
  &__title {
    font-family: DM Serif Display;
    font-size: 65px;
    font-weight: 400;
    line-height: 81px;
    letter-spacing: 0em;
    text-align: left;
  }
  &__text {
    font-family: Jost;
    font-size: 22px;
    font-weight: 400;
    line-height: 33px;
    letter-spacing: 0.01em;
    text-align: left;
  }

  background-image: url(../assets/img/top_background.png);
  background-size: cover;
}
.projects {
  display: flex;
  flex-direction: column;
  align-content: center;
  align-items: center;
  flex-wrap: wrap;
  &__heading {
    padding-top: 50px;
    &_title {
      font-family: DM Serif Display;
      font-size: 50px;
      font-weight: 400;
      line-height: 63px;
      letter-spacing: 0.02em;
      text-align: center;
    }
    &_text {
      font-family: Jost;
      font-size: 22px;
      font-weight: 400;
      line-height: 33px;
      letter-spacing: 0.01em;
      text-align: center;
    }
  }
  &__catalog {
    width: 1201px;
    display: flex;
    flex-wrap: wrap;
    &_box {
      display: flex;
      flex-wrap: wrap;
      gap: 40px;
      justify-content: center;
    }
  }
  &__item {
    width: 525px;
    height: 548px;
  }
}
.middle {
  background-color: #f4f0ec;
  display: flex;
  position: relative;
  justify-content: center;
  text-align: center;
  align-items: center;
  width: 100%;
  height: 457px;
  margin-top: 50px;
  &__item {
    display: flex;
    flex-direction: column;
    justify-content: center;
    border-left: 1px solid #cda274;
    border-right: 1px solid #cda274;
    width: 246px;
    height: 155px;
    align-items: center;

    &_title {
      font-family: DM Serif Display;
      font-size: 85px;
      font-weight: 400;
      line-height: 106px;
      letter-spacing: 0.02em;
      text-align: left;
      color: #cda274;
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
.down {
  margin-top: 50px;
  &__heading {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    text-align: center;
    &_title {
      font-family: DM Serif Display;
      font-size: 50px;
      font-weight: 400;
      line-height: 63px;
      letter-spacing: 0.02em;
      text-align: center;
    }
    &_text {
      font-family: Jost;
      font-size: 22px;
      font-weight: 400;
      line-height: 33px;
      letter-spacing: 0.01em;
      text-align: center;
    }
  }
  &__items {
    display: flex;
    justify-content: center;
    margin-top: 30px;
  }
  &__item {
    width: 382px;
    height: 521px;
    &_img {
      border-radius: 10% 10% 0% 0%;
    }
    &_title {
      font-family: DM Serif Display;
      font-size: 25px;
      font-weight: 400;
      line-height: 31px;
      letter-spacing: 0.02em;
      text-align: left;
    }
    &_text {
      font-family: Jost;
      font-size: 16px;
      font-weight: 400;
      line-height: 24px;
      letter-spacing: 0.01em;
      text-align: left;
    }
  }
}

</style>
