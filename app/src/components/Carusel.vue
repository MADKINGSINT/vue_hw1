<template>
    <div>
        <div class="slider">
            <div class="slider__box" v-if="currentSlide ===0">
                <img class="slider__photo" src="../assets/img/Slider.png" alt="">
                <h1 class="slider__title">Slide 1</h1>
            </div>
            <div class="slider__box" v-if="currentSlide ===1">
                             <img class="slider__photo" src="../assets/img/Slider.png" alt="">
                <h1 class="slider__title">Slide 2</h1>
            </div>
            <div class="slider__box" v-if="currentSlide ===2">
                             <img class="slider__photo" src="../assets/img/Slider.png" alt="">
                <h1 class="slider__title">Slide 3</h1>
            </div>
            <nav class="slider__circles">
                <button class="slider__circle" v-on:click="changeSlide(0)">o</button>
                <button class="slider__circle" v-on:click="changeSlide(1)">o</button>
                <button class="slider__circle" v-on:click="changeSlide(2)">o</button>
            </nav>
            <nav class="slider__btns">
            
                    <button class="slider__nav" v-on:click="nextSlide(currentSLide)">Вперед</button>
                    <button class="slider__nav" v-on:click="prevSlide(currentSlide)">Назад</button>
            </nav>
        </div>
    </div>
</template>

<script>
    export default {
        data() {
            return {
                currentSlide: 0,
            }
    },
    methods: {
        nextSlide(currentSlide) {
            if (this.currentSlide !== 2){ this.currentSlide += 1; }
            
        },
        prevSlide(CurrentSlide) {

            if (this.currentSlide!==0){ this.currentSlide -= 1;}
        },
        changeSlide(slide) {
            this.currentSlide = slide;
        }
    },
        
    }
</script>

<style lang="scss" scoped>
    .slider{
        display: flex;
        flex-direction: column;
        align-content: center;
        align-items: center;
        &__photo{
            border-radius: 20%;
        }

        &__title{
            justify-content: center;
        }
        &__box{
            display: flex;
            flex-direction: column;
            align-content: center;
            align-items: center;
        }
        &__circle{
            width: 20px;
            height: 20px;
            border-radius: 40%;
        }
    }
</style>