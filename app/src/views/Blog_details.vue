<template>
  <div class="top-banner">
    <div class="top-banner__content"></div>
  </div>
  <div class="blog-details center">
    <div class="blog-details__content">
      <article v-for="article in currentArticle" :key="article.id" class="article">
        <div class="article__content">
          <h2 class="article__heading">{{ article.firstheading }}</h2>
          <img class="article__image" :src="article.src" :alt="article.alt" />
          <div class="article__subcontent">
            <p class="article__date">
              {{ article.date }}
            </p>
            <div class="breadcrumbs">
              <ul class="breadcrumbs__list">
                <li class="breadcrumbs__item">
                  <a href="#" class="breadcrumbs__link">
                    {{ article.firstlink }}
                  </a>
                </li>
                <li class="breadcrumbs__item">
                  <a href="#" class="breadcrumbs__link">
                    {{ article.secondlink }}
                  </a>
                </li>
                <li class="breadcrumbs__item">
                  <a href="#" class="breadcrumbs__link">
                    {{ article.thirdlink }}
                  </a>
                </li>
              </ul>
            </div>
          </div>
          <p class="article__text">{{ article.firstparagraph }}</p>
          <p class="article__text">{{ article.secondparagraph }}</p>
        </div>
        <div class="quotes">
          <div class="quotes__content">
            <div class="quotes__marks">
              <svg
                width="74"
                height="56"
                viewBox="0 0 74 56"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  d="M58.2516 0.600003C62.6516 0.600003 66.2516 2.06667 69.0516 5C71.7182 7.93334 73.0516 11.8667 73.0516 16.8C73.0516 25.4667 70.1849 33 64.4516 39.4C58.5849 45.8 51.5849 51.0667 43.4516 55.2L41.4516 51.8C44.7849 49.6667 47.9182 46.9333 50.8516 43.6C53.6516 40.2667 55.8516 36.6667 57.4516 32.8L51.8516 28.6C49.5849 27.1333 47.7182 25.1333 46.2516 22.6C44.7849 20.2 44.0516 17.8667 44.0516 15.6C44.0516 11.3333 45.3849 7.73334 48.0516 4.8C50.5849 2 53.9849 0.600002 58.2516 0.600003ZM17.0516 0.599999C21.4516 0.6 25.0516 2.06667 27.8516 5C30.5182 7.93333 31.8516 11.8667 31.8516 16.8C31.8516 25.4667 28.9849 33 23.2516 39.4C17.3849 45.8 10.3849 51.0667 2.25155 55.2L0.251554 51.8C3.58489 49.6667 6.71822 46.9333 9.65155 43.6C12.4516 40.2667 14.6516 36.6667 16.2516 32.8L10.6516 28.6C8.38489 27.1333 6.51822 25.1333 5.05155 22.6C3.58489 20.2 2.85156 17.8667 2.85156 15.6C2.85156 11.3333 4.18489 7.73333 6.85156 4.8C9.38489 2 12.7849 0.599999 17.0516 0.599999Z"
                  fill="#CDA274"
                />
              </svg>
            </div>
            <p class="quotes__text">{{ article.quotetext }}</p>
          </div>
        </div>
        <h2 class="article__heading">{{ article.secondheading }}</h2>
        <p class="article__text">{{ article.thirdparagraph }}</p>
        <div class="article__subtext-box">
          <span class="article__subtext-span">{{ article.firstspan }}</span>
          <p class="article__subtext">{{ article.firstsubtext }}</p>
        </div>
        <div class="article__subtext-box">
          <span class="article__subtext-span">{{ article.secondspan }}</span>
          <p class="article__subtext">{{ article.secondsubtext }}</p>
        </div>
        <div class="article__subtext-box">
          <span class="article__subtext-span">{{ article.thirdspan }}</span>
          <p class="article__subtext">{{ article.thirdsubtext }}</p>
        </div>
        <img class="article__image" :src="article.secondsrc" :alt="article.secondalt" />
        <p class="article__text">{{ article.forthparagraph }}</p>
      </article>
      <aside class="sidebar">
        <div class="sidebar__content">
          <h3 class="sidebar__heading">{{ sidebarTitle }}</h3>
          <div class="sidebar__buttons-box">
            <button
              v-for="button in buttons"
              :key="button.id"
              @click="changeArticle(button.id)"
              type="button"
              :class="[
                'sidebar__button',
                button.id === buttonIsActive ? 'sidebar__button_active' : false,
              ]"
            >
              {{ button.title }}
            </button>
          </div>
        </div>
      </aside>
    </div>
  </div>
</template>

<script>
export default {
  name: "BlogDetails",
  data() {
    return {
      currentArticle: [
        {
          id: "kitchen",
          firstheading: "Let’s Get Solution for Building Construction Work",
          src: require("@/assets/img/article_img.png"),
          alt: "kitchen",
          date: "26 December,2022",
          firstlink: "Interior",
          secondlink: "Home",
          thirdlink: "Decore",
          firstparagraph:
            "Lorem ipsum dolor sit amet, adipiscing Aliquam eu sem vitae turpmaximus.posuere in.Contrary to popular belief.There are many variations of passages of Lorem Ipsum available, but the majority have suffered alteration in some form, by injecthumour.",
          secondparagraph:
            "Embarrassing hidden in the middle of text. All the Lorem Ipsum generators on the Internet tend to repeat predefined chunks as necessary.",
          quotetext: "The details are not the details. They make the design.",
          secondheading: "Design sprints are great",
          thirdparagraph:
            "Lorem ipsum dolor sit amet, adipiscing Aliquam eu sem vitae turpmaximus.posuere in.Contrary to popular belief.There are many variations of passages of Lorem Ipsum available, but the majority have suffered.",
          firstspan: "1",
          firstsubtext:
            "Contrary to popular belief.There are many variations of passages of Lorem Ipsum available, but the majority have suffered.",
          secondspan: "2",
          secondsubtext:
            "Contrary to popular belief.There are many variations of passages of Lorem Ipsum available, but the majority have suffered.",
          thirdspan: "3",
          thirdsubtext:
            "Contrary to popular belief.There are many variations of passages of Lorem Ipsum available, but the majority have suffered.",
          secondsrc: require("@/assets/img/article_img.png"),
          secondalt: "kitchen image",
          forthparagraph:
            "Contrary to popular belief.There are many variations of passages of Lorem Ipsum available, but the majority have suffered.",
        },
      ],
      listOfArticles: [
        {
          id: "kitchen",
          firstheading: "Let’s Get Solution for Building Construction Work",
          src: require("@/assets/img/article_img.png"),
          alt: "kitchen",
          date: "26 December,2022",
          firstlink: "Interior",
          secondlink: "Home",
          thirdlink: "Decore",
          firstparagraph:
            "Lorem ipsum dolor sit amet, adipiscing Aliquam eu sem vitae turpmaximus.posuere in.Contrary to popular belief.There are many variations of passages of Lorem Ipsum available, but the majority have suffered alteration in some form, by injecthumour.",
          secondparagraph:
            "Embarrassing hidden in the middle of text. All the Lorem Ipsum generators on the Internet tend to repeat predefined chunks as necessary.",
          quotetext: "The details are not the details. They make the design.",
          secondheading: "Design sprints are great",
          thirdparagraph:
            "Lorem ipsum dolor sit amet, adipiscing Aliquam eu sem vitae turpmaximus.posuere in.Contrary to popular belief.There are many variations of passages of Lorem Ipsum available, but the majority have suffered.",
          firstspan: "1",
          firstsubtext:
            "Contrary to popular belief.There are many variations of passages of Lorem Ipsum available, but the majority have suffered.",
          secondspan: "2",
          secondsubtext:
            "Contrary to popular belief.There are many variations of passages of Lorem Ipsum available, but the majority have suffered.",
          thirdspan: "3",
          thirdsubtext:
            "Contrary to popular belief.There are many variations of passages of Lorem Ipsum available, but the majority have suffered.",
          secondsrc: require("@/assets/img/article_img.png"),
          secondalt: "kitchen image",
          forthparagraph:
            "Contrary to popular belief.There are many variations of passages of Lorem Ipsum available, but the majority have suffered.",
        },
        {
          id: "bedroom",
          firstheading:
            "A bedroom or bedchamber is a room situated within a residential or accommodation unit characterised by its usage for sleeping",
          src: require("@/assets/img/article_img.png"),
          alt: "bedroom",
          date: "26 December,2022",
          firstlink: "Interior",
          secondlink: "Home",
          thirdlink: "Bedroom",
          firstparagraph:
            "Lorem ipsum dolor sit amet, adipiscing Aliquam eu sem vitae turpmaximus.posuere in.Contrary to popular belief.There are many variations of passages of Lorem Ipsum available, but the majority have suffered alteration in some form, by injecthumour, or randomised words which don't look even slightly believable.",
          secondparagraph:
            "Embarrassing hidden in the middle of text. All the Lorem Ipsum generators on the Internet tend to repeat predefined chunks as necessary.",
          quotetext: "The details are not the details. They make the design.",
          secondheading: "Design sprints are great",
          thirdparagraph:
            "Lorem ipsum dolor sit amet, adipiscing Aliquam eu sem vitae turpmaximus.posuere in.Contrary to popular belief.There are many variations of passages of Lorem Ipsum available, but the majority have suffered.",
          firstspan: "1",
          firstsubtext:
            "Contrary to popular belief.There are many variations of passages of Lorem Ipsum available, but the majority have suffered.",
          secondspan: "2",
          secondsubtext:
            "Contrary to popular belief.There are many variations of passages of Lorem Ipsum available, but the majority have suffered.",
          thirdspan: "3",
          thirdsubtext:
            "Contrary to popular belief.There are many variations of passages of Lorem Ipsum available, but the majority have suffered.",
          secondsrc: require("@/assets/img/article_img.png"),
          secondalt: "bedroom image",
          forthparagraph:
            "Contrary to popular belief.There are many variations of passages of Lorem Ipsum available, but the majority have suffered.",
        },
        {
          id: "building",
          firstheading:
            "A building is 'a structure that has a roof and walls and stands more or less permanently in one place",
          src: require("@/assets/img/article_img.png"),
          alt: "building",
          date: "26 December,2022",
          firstlink: "Interior",
          secondlink: "Home",
          thirdlink: "Building",
          firstparagraph:
            "Lorem ipsum dolor sit amet, adipiscing Aliquam eu sem vitae turpmaximus.posuere in.Contrary to popular belief.There are many variations of passages of Lorem Ipsum available, but the majority have suffered alteration in some form, by injecthumour, or randomised words which don't look even slightly believable.",
          secondparagraph:
            "Embarrassing hidden in the middle of text. All the Lorem Ipsum generators on the Internet tend to repeat predefined chunks as necessary.",
          quotetext: "The details are not the details. They make the design.",
          secondheading: "Design sprints are great",
          thirdparagraph:
            "Lorem ipsum dolor sit amet, adipiscing Aliquam eu sem vitae turpmaximus.posuere in.Contrary to popular belief.There are many variations of passages of Lorem Ipsum available, but the majority have suffered.",
          firstspan: "1",
          firstsubtext:
            "Contrary to popular belief.There are many variations of passages of Lorem Ipsum available, but the majority have suffered.",
          secondspan: "2",
          secondsubtext:
            "Contrary to popular belief.There are many variations of passages of Lorem Ipsum available, but the majority have suffered.",
          thirdspan: "3",
          thirdsubtext:
            "Contrary to popular belief.There are many variations of passages of Lorem Ipsum available, but the majority have suffered.",
          secondsrc: require("@/assets/img/article_img.png"),
          secondalt: "building image",
          forthparagraph:
            "Contrary to popular belief.There are many variations of passages of Lorem Ipsum available, but the majority have suffered.",
        },
        {
          id: "architecture",
          firstheading:
            "Architecture is the art and technique of designing and building, as distinguished from the skills associated with construction",
          src: require("@/assets/img/article_img.png"),
          alt: "architecture",
          date: "26 December,2022",
          firstlink: "Interior",
          secondlink: "Home",
          thirdlink: "Architecture",
          firstparagraph:
            "Lorem ipsum dolor sit amet, adipiscing Aliquam eu sem vitae turpmaximus.posuere in.Contrary to popular belief.There are many variations of passages of Lorem Ipsum available, but the majority have suffered alteration in some form, by injecthumour, or randomised words which don't look even slightly believable.",
          secondparagraph:
            "Embarrassing hidden in the middle of text. All the Lorem Ipsum generators on the Internet tend to repeat predefined chunks as necessary.",
          quotetext: "The details are not the details. They make the design.",
          secondheading: "Design sprints are great",
          thirdparagraph:
            "Lorem ipsum dolor sit amet, adipiscing Aliquam eu sem vitae turpmaximus.posuere in.Contrary to popular belief.There are many variations of passages of Lorem Ipsum available, but the majority have suffered.",
          firstspan: "1",
          firstsubtext:
            "Contrary to popular belief.There are many variations of passages of Lorem Ipsum available, but the majority have suffered.",
          secondspan: "2",
          secondsubtext:
            "Contrary to popular belief.There are many variations of passages of Lorem Ipsum available, but the majority have suffered.",
          thirdspan: "3",
          thirdsubtext:
            "Contrary to popular belief.There are many variations of passages of Lorem Ipsum available, but the majority have suffered.",
          secondsrc: require("@/assets/img/article_img.png"),
          secondalt: "architecture image",
          forthparagraph:
            "Contrary to popular belief.There are many variations of passages of Lorem Ipsum available, but the majority have suffered.",
        },
        {
          id: "kitchen-planning",
          firstheading:
            "A kitchen is a room or part of a room used for cooking and food preparation in a dwelling or in a commercial establishment",
          src: require("@/assets/img/article_img.png"),
          alt: "kitchen-planning",
          date: "26 December,2022",
          firstlink: "Interior",
          secondlink: "Home",
          thirdlink: "Kitchen planning",
          firstparagraph:
            "Lorem ipsum dolor sit amet, adipiscing Aliquam eu sem vitae turpmaximus.posuere in.Contrary to popular belief.There are many variations of passages of Lorem Ipsum available, but the majority have suffered alteration in some form, by injecthumour, or randomised words which don't look even slightly believable.",
          secondparagraph:
            "Embarrassing hidden in the middle of text. All the Lorem Ipsum generators on the Internet tend to repeat predefined chunks as necessary.",
          quotetext: "The details are not the details. They make the design.",
          secondheading: "Design sprints are great",
          thirdparagraph:
            "Lorem ipsum dolor sit amet, adipiscing Aliquam eu sem vitae turpmaximus.posuere in.Contrary to popular belief.There are many variations of passages of Lorem Ipsum available, but the majority have suffered.",
          firstspan: "1",
          firstsubtext:
            "Contrary to popular belief.There are many variations of passages of Lorem Ipsum available, but the majority have suffered.",
          secondspan: "2",
          secondsubtext:
            "Contrary to popular belief.There are many variations of passages of Lorem Ipsum available, but the majority have suffered.",
          thirdspan: "3",
          thirdsubtext:
            "Contrary to popular belief.There are many variations of passages of Lorem Ipsum available, but the majority have suffered.",
          secondsrc: require("@/assets/img/article_img.png"),
          secondalt: "kitchen-planning image",
          forthparagraph:
            "Contrary to popular belief.There are many variations of passages of Lorem Ipsum available, but the majority have suffered.",
        },
      ],
      sidebarTitle: "Tags",
      buttons: [
        { id: "kitchen", title: "Kitchen" },
        { id: "bedroom", title: "Bedroom" },
        { id: "building", title: "Building" },
        { id: "architecture", title: "Architecture" },
        { id: "kitchen-planning", title: "Kitchen Planning" },
      ],
      buttonIsActive: "kitchen",
    };
  },
  methods: {
    changeArticle(id) {
      const buttonId = id;
      this.listOfArticles.forEach((article) => {
        if (buttonId === article.id) {
          this.currentArticle = [];
          this.buttonIsActive = id;
          return this.currentArticle.push(article);
        }
      });
    },
  },
};
</script>

<style lang="scss">
$mainColorOfSite: #ffffff;
$lightColor: #e7e7e7;
$firstPrimaryColor: #cda274;
$secondPrimaryColor: #292f36;
$thirdPrimaryColor: #f4f0ec;
$fourthPrimaryColor: #4d5053;
$desktopWidthOfSite: 1200px;

@mixin transition-fast() {
  transition: all 0.5s ease-out;
}

@mixin transition-slow() {
  transition: all 0.8s ease-out;
}

@mixin font-jost-regular($color, $size, $height) {
  color: $color;
  font-family: "Jost", sans-serif;
  font-weight: 400;
  font-style: normal;
  font-size: $size;
  line-height: $height;
}

@mixin font-jost-medium($color, $size, $height) {
  color: $color;
  font-family: "Jost", sans-serif;
  font-weight: 500;
  font-style: normal;
  font-size: $size;
  line-height: $height;
}

@mixin font-jost-semibold($color, $size, $height) {
  color: $color;
  font-family: "Jost", sans-serif;
  font-weight: 600;
  font-style: normal;
  font-size: $size;
  line-height: $height;
}

@mixin font-DMSerifDisplay-regular($color, $size, $height) {
  color: $color;
  font-family: " DM Serif Display", sans-serif;
  font-weight: 400;
  font-style: normal;
  font-size: $size;
  line-height: $height;
}

@mixin font-DMSerifDisplay-semibold($color, $size, $height) {
  color: $color;
  font-family: " DM Serif Display", sans-serif;
  font-weight: 600;
  font-style: normal;
  font-size: $size;
  line-height: $height;
}

.top-banner {
  margin-bottom: 200px;

  &__content {
    background-image: url("../assets/img/article_img.png");
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
    display: flex;
    justify-content: center;
    height: 356px;
  }
}

.blog-details {
  margin-bottom: 96px;

  &__content {
    display: grid;
    grid-template-columns: 799px 345px;
    justify-content: center;
    align-items: flex-start;
    gap: 52px;
  }
}

.article {
  &__heading {
    @include font-DMSerifDisplay-regular($secondPrimaryColor, 50px, 1.25);
    letter-spacing: 1px;
    margin: 0;
    margin-bottom: 21px;
  }

  &__image {
    margin-bottom: 46px;
  }

  &__subcontent {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: flex-start;
    margin-bottom: 48px;
  }

  &__date {
    @include font-jost-regular($fourthPrimaryColor, 16px, 1.5);
    letter-spacing: 0.16px;
    text-transform: capitalize;
    margin: 0;
  }

  &__text {
    @include font-jost-regular($fourthPrimaryColor, 22px, 1.5);
    letter-spacing: 0.22px;
    margin: 0;
    margin-bottom: 35px;

    &:nth-child(3) {
      margin-bottom: 24px;
    }
  }

  &__subtext-box {
    display: flex;
    flex-direction: row;
    justify-content: flex-start;
    align-items: flex-start;
    gap: 14px;
    margin-bottom: 32px;

    &:nth-child(3) {
      margin-bottom: 44px;
    }
  }

  &__subtext-span {
    @include font-DMSerifDisplay-regular($firstPrimaryColor, 20px, 1.25);
    letter-spacing: 0.4px;
    margin: 0;
  }

  &__subtext {
    @include font-jost-regular($fourthPrimaryColor, 22px, 1.5);
    letter-spacing: 0.22px;
    margin: 0;
  }
}

.breadcrumbs {
  &__list {
    display: flex;
    flex-direction: row;
    justify-content: center;
    margin: 0;
  }

  &__item {
    &:not(:last-child)::after {
      content: "/";
      margin-left: 8px;
      margin-right: 8px;
    }
  }

  &__link {
    @include font-jost-regular($fourthPrimaryColor, 16px, 1.5);
    letter-spacing: 0.16px;
    text-transform: capitalize;
    margin: 0;
    @include transition-fast();

    &:hover {
      color: $firstPrimaryColor;
      @include transition-slow();
    }

    &:active {
      color: $fourthPrimaryColor;
      @include transition-slow();
    }

    &:focus {
      color: $firstPrimaryColor;
      @include transition-slow();
    }
  }
}

.quotes {
  margin-bottom: 27px;

  &__content {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    padding: 53px 200px;
    border-radius: 50px;
    background: $thirdPrimaryColor;
  }

  &__text {
    @include font-DMSerifDisplay-regular($firstPrimaryColor, 25px, 1.25);
    text-align: center;
    font-style: italic;
    letter-spacing: 0.5px;
    margin: 0;
  }
}

.sidebar {
  &__content {
    display: flex;
    flex-direction: column;
    justify-content: flex-start;
    align-items: flex-start;
    gap: 24px;
  }

  &__heading {
    @include font-DMSerifDisplay-regular($secondPrimaryColor, 25px, 1.25);
    letter-spacing: 0.5px;
    margin: 0;
  }

  &__buttons-box {
    display: flex;
    justify-content: flex-start;
    align-content: flex-start;
    flex-wrap: wrap;
    gap: 10px;
  }

  &__button {
    @include font-jost-regular($secondPrimaryColor, 18px, 1.25);
    letter-spacing: 0.36px;
    border: none;
    border-radius: 10px;
    background-color: $thirdPrimaryColor;
    padding: 9px 30px;
    @include transition-fast();

    &:hover {
      background-color: $firstPrimaryColor;
      @include transition-slow();
    }

    &:focus {
      color: $mainColorOfSite;
      background-color: $secondPrimaryColor;
      @include transition-slow();
    }
  }

  &__button_active {
    color: $mainColorOfSite;
    background-color: $secondPrimaryColor;
  }
}
</style>
