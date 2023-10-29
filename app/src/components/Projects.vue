<template>
    <div>
        <div class="hheading">
            <div class="hheading__box">
                <h1 class="hheading__box"></h1>
                <p class="hheading__text"></p>
            </div>
        </div>
    </div>
        <nav class="project__nav">
            <button v-on:click="this.currentList = 0" class="project__nav_btn">Bedroom</button>
            <button v-on:click="this.currentList = 1" class="project__nav_btn">Bathroom</button>
            <button v-on:click="this.currentList = 2" class="project__nav_btn">Kitchen</button>
            <button v-on:click="this.currentList = 3" class="project__nav_btn">Living Area</button>
        </nav>
    <div class="project">

        <div class="project__box1">
            <div v-if="currentList ===0">
                    <img class="project__box1_star" src="../assets/img/Star.svg" alt="">
                    <img :src="Bedroom.src1" alt="">
                    <h3 class="project__title">{{Bedroom.h3}}</h3>
                    <p class="project__text">{{Bedroom.text}}</p>
                    <img class="project__box1_star" src="../assets/img/Star.svg" alt="">
                    <img :src="Bedroom.src2" alt="">
                    <h3 class="project__title">{{Bedroom.h3}}</h3>
                    <p class="project__text">{{Bedroom.text}}</p>
                    <img class="project__box1_star" src="../assets/img/Star.svg" alt="">
                    <img :src="Bedroom.src1" alt="">
                    <h3 class="project__title">{{Bedroom.h3}}</h3>
                    <p class="project__text">{{Bedroom.text}}</p>
                    <img class="project__box1_star" src="../assets/img/Star.svg" alt="">
                    <img :src="Bedroom.src2" alt="">
                    <h3 class="project__title">{{Bedroom.h3}}</h3>
                    <p class="project__text">{{Bedroom.text}}</p>
            
                
            </div>
                        <div v-if="currentList ===1">
                
                    <img :src="Bathroom.src1" alt="">
                    <img class="project__box1_star" src="../assets/img/Star.svg" alt="">
                    <h3 class="project__title">{{Bathroom.h3}}</h3>
                    <p class="project__text">{{Bathroom.text}}</p>
                    <img :src="Bathroom.src2" alt="">
                    <img class="project__box1_star" src="../assets/img/Star.svg" alt="">
                    <h3 class="project__title">{{Bathroom.h3}}</h3>
                    <p class="project__text">{{Bathroom.text}}</p>
                    <img :src="Bathroom.src1" alt="">
                    <img class="project__box1_star" src="../assets/img/Star.svg" alt="">
                    <h3 class="project__title">{{Bathroom.h3}}</h3>
                    <p class="project__text">{{Bathroom.text}}</p>
                    <img :src="Bathroom.src2" alt="">
                    <img class="project__box1_star" src="../assets/img/Star.svg" alt="">
                    <h3 class="project__title">{{Bathroom.h3}}</h3>
                    <p class="project__text">{{Bathroom.text}}</p>
            
                
            </div>
                        
                        <div v-if="currentList ===2">
                <img class="project__box1_star" src="../assets/img/Star.svg" alt="">
                    <img :src="Kitchen.src1" alt="">
                    
                    <h3 class="project__title">{{Kitchen.h3}}</h3>
                    <p class="project__text">{{Kitchen.text}}</p>
                    <img class="project__box1_star" src="../assets/img/Star.svg" alt="">
                    <img :src="Kitchen.src2" alt="">
                    <h3 class="project__title">{{Kitchen.h3}}</h3>
                    <p class="project__text">{{Kitchen.text}}</p>
                    <img class="project__box1_star" src="../assets/img/Star.svg" alt="">
                    <img :src="Kitchen.src1" alt="">
                    <h3 class="project__title">{{Kitchen.h3}}</h3>
                    <p class="project__text">{{Kitchen.text}}</p>
                    <img class="project__box1_star" src="../assets/img/Star.svg" alt="">
                    <img :src="Kitchen.src2" alt="">
                    <h3 class="project__title">{{Kitchen.h3}}</h3>
                    <p class="project__text">{{Kitchen.text}}</p>
            
                
            </div>
        
                                   <div v-if="currentList ===3">
                <img class="project__box1_star" src="../assets/img/Star.svg" alt="">
                    <img :src="LivingArea.src1" alt="">
                    <h3 class="project__title">{{LivingArea.h3}}</h3>
                    <p class="project__text">{{LivingArea.text}}</p>
                    <img class="project__box1_star" src="../assets/img/Star.svg" alt="">
                    <img :src="LivingArea.src2" alt="">
                    <h3 class="project__title">{{LivingArea.h3}}</h3>
                    <p class="project__text">{{LivingArea.text}}</p>
                    <img class="project__box1_star" src="../assets/img/Star.svg" alt="">
                    <img :src="LivingArea.src1" alt="">
                    <h3 class="project__title">{{LivingArea.h3}}</h3>
                    <p class="project__text">{{LivingArea.text}}</p>
                    <img class="project__box1_star" src="../assets/img/Star.svg" alt="">
                    <img :src="LivingArea.src2" alt="">
                    <h3 class="project__title">{{LivingArea.h3}}</h3>
                    <p class="project__text">{{LivingArea.text}}</p>
            
                
            </div>
                                  
   
   
   
 
            
            

        </div>
        <div class="project__box2">
                <div v-if="currentList ===0">
                <img class="project__box2_star" src="../assets/img/Star.svg" alt="">
                    <img :src="Bedroom.src2" alt="">
                    <h3 class="project__title">{{Bedroom.h3}}</h3>
                    <p class="project__text">{{Bedroom.text}}</p>
                    <img class="project__box2_star" src="../assets/img/Star.svg" alt="">
                    <img :src="Bedroom.src1" alt="">
                    <h3 class="project__title">{{Bedroom.h3}}</h3>
                    <p class="project__text">{{Bedroom.text}}</p>
                    <img class="project__box2_star" src="../assets/img/Star.svg" alt="">
                    <img :src="Bedroom.src2" alt="">
                    <h3 class="project__title">{{Bedroom.h3}}</h3>
                    <p class="project__text">{{Bedroom.text}}</p>
                    <img class="project__box2_star" src="../assets/img/Star.svg" alt="">
                    <img :src="Bedroom.src2" alt="">
                    <h3 class="project__title">{{Bedroom.h3}}</h3>
                    <p class="project__text">{{Bedroom.text}}</p>
            
                
            </div>
                            <div v-if="currentList ===1">
                <img class="project__box2_star" src="../assets/img/Star.svg" alt="">
                    <img :src="Bathroom.src2" alt="">
                    <h3 class="project__title">{{Bathroom.h3}}</h3>
                    <p class="project__text">{{Bathroom.text}}</p>
                    <img class="project__box2_star" src="../assets/img/Star.svg" alt="">
                    <img :src="Bathroom.src1" alt="">
                    <h3 class="project__title">{{Bathroom.h3}}</h3>
                    <p class="project__text">{{Bathroom.text}}</p>
                    <img class="project__box2_star" src="../assets/img/Star.svg" alt="">
                    <img :src="Bathroom.src2" alt="">
                    <h3 class="project__title">{{Bathroom.h3}}</h3>
                    <p class="project__text">{{Bathroom.text}}</p>
                    <img class="project__box2_star" src="../assets/img/Star.svg" alt="">
                    <img :src="Bathroom.src2" alt="">
                    <h3 class="project__title">{{Bathroom.h3}}</h3>
                    <p class="project__text">{{Bathroom.text}}</p>
            
                
            </div>
                       <div v-if="currentList ===2">
                <img class="project__box2_star" src="../assets/img/Star.svg" alt="">
                    <img :src="Kitchen.src2" alt="">
                    <h3 class="project__title">{{Kitchen.h3}}</h3>
                    <p class="project__text">{{Kitchen.text}}</p>
                    <img class="project__box2_star" src="../assets/img/Star.svg" alt="">
                    <img :src="Kitchen.src1" alt="">
                    <h3 class="project__title">{{Kitchen.h3}}</h3>
                    <p class="project__text">{{Kitchen.text}}</p>
                    <img class="project__box2_star" src="../assets/img/Star.svg" alt="">
                    <img :src="Kitchen.src2" alt="">
                    <h3 class="project__title">{{Kitchen.h3}}</h3>
                    <p class="project__text">{{Kitchen.text}}</p>
                    <img class="project__box2_star" src="../assets/img/Star.svg" alt="">
                    <img :src="Kitchen.src2" alt="">
                    <h3 class="project__title">{{Kitchen.h3}}</h3>
                    <p class="project__text">{{Kitchen.text}}</p>
            
                
            </div>
              <div v-if="currentList ===3">
                <img class="project__box2_star" src="../assets/img/Star.svg" alt="">
                    <img :src="LivingArea.src2" alt="">
                    <h3 class="project__title">{{LivingArea.h3}}</h3>
                    <p class="project__text">{{LivingArea.text}}</p>
                    <img class="project__box2_star" src="../assets/img/Star.svg" alt="">
                    <img :src="LivingArea.src1" alt="">
                    <h3 class="project__title">{{LivingArea.h3}}</h3>
                    <p class="project__text">{{LivingArea.text}}</p>
                    <img class="project__box2_star" src="../assets/img/Star.svg" alt="">
                    <img :src="LivingArea.src2" alt="">
                    <h3 class="project__title">{{LivingArea.h3}}</h3>
                    <p class="project__text">{{LivingArea.text}}</p>
                    <img class="project__box2_star" src="../assets/img/Star.svg" alt="">
                    <img :src="LivingArea.src2" alt="">
                    <h3 class="project__title">{{LivingArea.h3}}</h3>
                    <p class="project__text">{{LivingArea.text}}</p>
            
                
            </div>
<!--                                     <img src="../assets/img/project.png" alt="">
            <h3 class="project__title">Minimal Bedroom</h3>
            <p class="project__text">Decor / Artchitecture</p>
            <button class="project__btn"><img src="../assets/img/strelka.svg" alt=""></button>
                        <img src="../assets/img/project_big.png" alt="">
            <h3 class="project__title">Minimal Bedroom</h3>
            <p class="project__text">Decor / Artchitecture</p>
            <button class="project__btn"><img src="../assets/img/strelka.svg" alt=""></button>
                        <img src="../assets/img/project.png" alt="">
            <h3 class="project__title">Minimal Bedroom</h3>
            <p class="project__text">Decor / Artchitecture</p>
            <button class="project__btn"><img src="../assets/img/strelka.svg" alt=""></button>
                        <img src="../assets/img/project.png" alt="">
            <h3 class="project__title">Minimal Bedroom</h3>
            <p class="project__text">Decor / Artchitecture</p>
            <button class="project__btn"><img src="../assets/img/strelka.svg" alt=""></button> -->

        </div>
    </div>
</template>

<script>
    export default {
    data() {
        return {
            currentList: 0,
            Bedroom: {
                
                src1: require("@/assets/img/project_big.png"),
                src2: require("@/assets/img/project.png"),

                h3: "Minimal Bedroom",
                text: "Decor / Artchitecture"

            },
            Bathroom: {

                               src1: require("@/assets/img/project_big.png"),
                src2: require("@/assets/img/project.png"),
                src3: require("@/assets/img/project_big.png"),
                src4: require("@/assets/img/project.png"),
                h3: "Minimal Bathroom",
                text: "Decor / Artchitecture"


            },
            Kitchen: {
                    
                                   src1: require("@/assets/img/project_big.png"),
                src2: require("@/assets/img/project.png"),
                src3: require("@/assets/img/project_big.png"),
                src4: require("@/assets/img/project.png"),
                    h3: "Minimal Kitchen",
                    text: "Decor / Artchitecture"
        
            },
            LivingArea: {

                               src1: require("@/assets/img/project_big.png"),
                src2: require("@/assets/img/project.png"),
                src3: require("@/assets/img/project_big.png"),
                src4: require("@/assets/img/project.png"),
                h3: "Minimal Livingroom",
                text: "Decor / Artchitecture"

            }

                
            }
        },
    }
</script>

<style lang="scss" scoped>
    .project{
        display: flex;
        
        justify-content: center;
        gap:  30px;
        &__nav{
            display: flex;
            justify-content: center;
            height:  80px;
            &_btn{
                width: 219px;
                height: 75px;
                border-radius: 18px; 
                background-color: white;
            }
            &_btn:hover{
                background-color: #CDA274; transition: 1s;
            }
        }
        &__title{
            color: #292F36;
            font-family: DM Serif Display;
            font-size: 25px;
            font-style: normal;
            font-weight: 400;
            line-height: 125%; /* 31.25px */
            letter-spacing: 0.5px;
        }
        &__text{
            color: #4D5053;
            font-family: Jost;
            font-size: 22px;
            font-style: normal;
            font-weight: 400;
            line-height: 150%; /* 33px */
            letter-spacing: 0.22px;
        }
        &__box1{
            display: flex;
            flex-direction: column;
            &_star{
                position: absolute;
                padding-left: 550px;
                cursor: pointer;

            }
            &_star:active{
                content: url(../assets/img/Gold_star.svg);
            }

        }
        &__box2{
            display: flex;
            flex-direction: column;
            &_star{
                position: absolute;
                padding-left: 550px;
            }
                        &_star:active{
                content: url(../assets/img/Gold_star.svg);
            }
        }
        &__btn{
            width: 70px;
            height:  70px;
            border-radius: 40px;
        }
    }
</style>
<!--             <img src="../assets/img/project_big.png" alt="">
            <h3 class="project__title">Minimal Bedroom</h3>
            <p class="project__text">Decor / Artchitecture</p>
            <button class="project__btn"><img src="../assets/img/strelka.svg" alt=""></button>
                        <img src="../assets/img/project.png" alt="">
            <h3 class="project__title">Minimal Bedroom</h3>
            <p class="project__text">Decor / Artchitecture</p>
            <button class="project__btn"><img src="../assets/img/strelka.svg" alt=""></button>
                        <img src="../assets/img/project_big.png" alt="">
            <h3 class="project__title">Minimal Bedroom</h3>
            <p class="project__text">Decor / Artchitecture</p>
            <button class="project__btn"><img src="../assets/img/strelka.svg" alt=""></button>
            <img src="../assets/img/project.png" alt="">
                        <h3 class="project__title">Minimal Bedroom</h3>
            <p class="project__text">Decor / Artchitecture</p>
            <button class="project__btn"><img src="../assets/img/strelka.svg" alt=""></button> -->
            