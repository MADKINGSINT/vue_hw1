 
<script>
  import article_img from '../assets/img/article_img.png'
export default {
 
    name: "Blog",

            
            data() {

                return {
                    items: [
                        {id: 0, src: '../assets/img/article_img.png', title: 'Let’s Get Solution For Building Construction Work', date: '26 December,2022 '},
                        {id: 1, src: "../assets/img/article_img.png", title: 'Let’s Get Solution For Building Construction Work', date: '26 December,2022 '},
                        {id: 2, src: '../assets/img/article_img.png', title: 'Let’s Get Solution For Building Construction Work', date: '26 December,2022 '},
                        {id: 3, src: '../assets/img/article_img.png', title: 'Let’s Get Solution For Building Construction Work', date: '26 December,2022 '},
                        {id: 4, src: '../assets/img/article_img.png', title: 'Let’s Get Solution For Building Construction Work', date: '26 December,2022 '},
                        {id: 5, src: '../assets/img/article_img.png', title: 'Let’s Get Solution For Building Construction Work', date: '26 December,2022 '}
                ],
                }
            },
        }
    

</script>

<template>
          
      <div id="blog">
            
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" href="style.css">
    <link href="https://fonts.googleapis.com/css2?family=DM+Serif+Display&family=Dancing+Script&family=Raleway:wght@100;400;500;600;700&display=swap" rel="stylesheet">
    <link rel="preconnect" href="https://fonts.googleapis.com">

    <link href="https://fonts.googleapis.com/css2?family=Jost&display=swap" rel="stylesheet">
    
</head>
<body>

    <section class="heading">
        <div class="heading__title center">
            <h1 class="heading__title_title">Articles & News</h1>
            <p class="heading__title_text">Home / Blog</p>
        </div>
    </section>
    <section class="post">
        <h1 class="post_heading">Latest Post</h1>
        <div class="post__item">
            <img class="post__item_img" src="../assets/img/post_img.png" alt="">
            <div class="post__post">

                <h2 class="post__item_title">Low Cost Latest Invented Interior Designing Ideas</h2>
                <p class="post__item_text">Lorem ipsum dolor sit amet, adipiscing Aliquam eu sem vitae turpis dignissim maximus.posuere in.Contrary to popular belief.

                    Lorem Ipsum is not simply random text. It has roots in a piece of classica.</p>
                    <div class="post__date">
                        <p class="post__date_date">26 December,2022 </p>
                        <button class="post__date_btn"><a href="#"><img src="../assets/img/strelka.svg" alt=""></a></button>
                    </div>
            </div>

        </div>
    </section>
    <article class="articles">
        <h1 class="articles__heading">Articles & News</h1>
        <div id="app">
<!--             <img v-for="item in items" :key="item.id" :src='item.src' alt="">
            <h1 v-for="item in items" :key="item.id">{{item.title}}</h1> -->
            <div class="articles__item" v-for="item in items" :key="item.id">
                <img class="articles__item_img" src="../assets/img/article_img.png" alt="">
                <h1 class="articles__item_title">{{item.title}}</h1>
                <span class="articles__item_date"><p class="articles__item_text">{{item.date}}</p>
                    <button class="articles__item_btn"><img src="../assets/img/strelka.svg" alt=""></button></span>
            </div>
        </div>

    </article>

    
</body>
</html>
      </div> 

    
</template>
<style lang="scss">
    .heading {
  background-image: url(../assets/img/heading.jpg);
  width: 100%;
  height: 356px;
  background-size: cover;
  display: flex;
  &__title {
    display: flex;
    width: 503px;
    height: 178px;
    position: absolute;
    flex-direction: column;
    align-items: center;
    gap: 10px;
    background-color: #fff;
    margin-left: 677px;
    margin-top: 200px;
    align-content: center;
    justify-content: center;
    border-radius: 20% 20% 0% 0%;
    &_title {
      color: #292f36;
      font-family: DM Serif Display;
      font-size: 50px;
      font-style: normal;
      font-weight: 400;
      line-height: 125%; /* 62.5px */
    }
    &_text {
      color: #4d5053;
      font-family: Jost;
      font-size: 22px;
      font-style: normal;
      font-weight: 400;
      line-height: 150%; /* 33px */
      letter-spacing: 0.22px;
    }
  }
}
.post {
  display: flex;
  flex-direction: column;
  &_heading {
    padding-top: 241px;
    color: #292f36;
    font-family: DM Serif Display;
    font-size: 50px;
    font-style: normal;
    font-weight: 400;
    line-height: 125%; /* 62.5px */
    letter-spacing: 1px;
    padding-left: 360px;
  }
  &__item {
    display: flex;
    &_img {
      margin-left: 339px;
      border-radius: 20%;
    }
    &_title {
      padding-left: 65px;
      width: 463px;
      color: #292f36;
      font-family: DM Serif Display;
      font-size: 25px;
      font-style: normal;
      font-weight: 400;
      line-height: 125%; /* 31.25px */
      letter-spacing: 0.5px;
    }
    &_text {
      padding-top: 22px;
      width: 469px;
      padding-left: 65px;
      color: #4d5053;
      font-family: Jost;
      font-size: 22px;
      font-style: normal;
      font-weight: 400;
      line-height: 150%; /* 33px */
      letter-spacing: 0.22px;
    }
  }
  &__post {
    display: flex;
    flex-direction: column;
  }
  &__date {
    padding-top: 50px;
    display: flex;
    gap: 50px;
    padding-left: 65px;
    &_date {
      color: #4d5053;
      font-family: Jost;
      font-size: 16px;
      font-style: normal;
      font-weight: 400;
      line-height: 150%; /* 24px */
      letter-spacing: 0.16px;
      text-transform: capitalize;
    }
    &_btn {
      width: 52px;
      height: 52px;
      border-radius: 50%;
      border-color: #292f36;
    }
  }
}
.articles {
  display: flex;
  justify-content: center;
  #app {
    margin-top: 100px;
    width: 1201px;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
  }
  &__item {
    width: 30%;
    &_img {
      border-radius: 15% 15% 0% 0%;
    }
    &_title {
      color: #292f36;
      font-family: DM Serif Display;
      font-size: 25px;
      font-style: normal;
      font-weight: 400;
      line-height: 125%; /* 31.25px */
      letter-spacing: 0.5px;
    }
    &_text {
      color: #4d5053;
      font-family: Jost;
      font-size: 16px;
      font-style: normal;
      font-weight: 400;
      line-height: 150%; /* 24px */
      letter-spacing: 0.16px;
      text-transform: capitalize;
    }
    &_date {
      display: flex;
      gap: 32px;
    }
    &_btn {
      width: 32px;
      height: 32px;
      border-radius: 50%;
    }
  }
  &__heading{
    color: #292F36;
    font-family: DM Serif Display;
    font-size: 50px;
    font-style: normal;
    font-weight: 400;
    line-height: 125%; /* 62.5px */
    letter-spacing: 1px;
    position: absolute;



  }
}
</style>