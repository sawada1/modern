<template>
    <div>
        <div class="mainteste">
      <h2>Testimonials</h2>
      <div class="Testimonials">
      <swiper
    :modules="modules"
    :slides-per-view="1"
    :space-between="50"
    navigation
    :pagination="{ clickable: true }"
    :scrollbar="{ draggable: true }"
    @swiper="onSwiper"
    @slideChange="onSlideChange"
    :autoplay="{
        delay: 3000,
     disableOnInteraction: false,
    }"
    
  >

    <swiper-slide>
      <div class=" boxx">
       <div class="image">
        <img src="../assets/img/testimonial/testimonial-1.jpg" alt="">
     
       </div>
       <div class="text">
        <h3>khaled sawada</h3>
        <span>web developer</span>
          <p>Lorem ipsum dolor sit amet consectetur
           adipisicing elit. Beatae, qui dolores
            praesentium laboriosam tempore suscipit iusto nisi eveniet fugit ea 
          molestiae cumque ullam neque minima at fugiat delectus architecto quibusdam!</p>
        </div>
      </div>
    </swiper-slide>
    <swiper-slide>
      <div class="container boxx">
       <div class="image">
        <img src="../assets/img/testimonial/testimonial-2.jpg" alt="">
     
       </div>
       <div class="text">
        <h3>khaled sawada</h3>
        <span>web developer</span>
          <p>Lorem ipsum dolor sit amet consectetur
           adipisicing elit. Beatae, qui dolores
            praesentium laboriosam tempore suscipit iusto nisi eveniet fugit ea 
          molestiae cumque ullam neque minima at fugiat delectus architecto quibusdam!</p>
        </div>
      </div>
    </swiper-slide>
    <swiper-slide>
      <div class="container boxx">
       <div class="image">
        <img src="../assets/img/testimonial/testimonial-3.jpg" alt="">
     
       </div>
       <div class="text">
        <h3>khaled sawada</h3>
        <span>web developer</span>
          <p>Lorem ipsum dolor sit amet consectetur
           adipisicing elit. Beatae, qui dolores
            praesentium laboriosam tempore suscipit iusto nisi eveniet fugit ea 
          molestiae cumque ullam neque minima at fugiat delectus architecto quibusdam!</p>
        </div>
      </div>
    </swiper-slide>
    <swiper-slide>
      <div class="container boxx">
       <div class="image">
        <img src="../assets/img/testimonial/testimonial-4.jpg" alt="">
     
       </div>
       <div class="text">
        <h3>khaled sawada</h3>
        <span>web developer</span>
          <p>Lorem ipsum dolor sit amet consectetur
           adipisicing elit. Beatae, qui dolores
            praesentium laboriosam tempore suscipit iusto nisi eveniet fugit ea 
          molestiae cumque ullam neque minima at fugiat delectus architecto quibusdam!</p>
        </div>
      </div>
    </swiper-slide>
    <swiper-slide>
      <div class="container boxx">
       <div class="image">
        <img src="../assets/img/testimonial/testimonial-5.jpg" alt="">
     
       </div>
       <div class="text">
        <h3>khaled sawada</h3>
        <span>web developer</span>
          <p>Lorem ipsum dolor sit amet consectetur
           adipisicing elit. Beatae, qui dolores
            praesentium laboriosam tempore suscipit iusto nisi eveniet fugit ea 
          molestiae cumque ullam neque minima at fugiat delectus architecto quibusdam!</p>
        </div>
      </div>
    </swiper-slide>
 

  </swiper>
    </div>
    </div>
    </div>
</template>

<script>
import {ref} from 'vue'
import { Navigation, Pagination, Scrollbar, A11y, Autoplay , EffectFade } from 'swiper';

// Import Swiper Vue.js components
import { Swiper, SwiperSlide } from 'swiper/vue';

// Import Swiper styles
import 'swiper/css';
import 'swiper/css/navigation';
import 'swiper/css/pagination';
import 'swiper/css/scrollbar';
export default {
   components:{
    Swiper,
      SwiperSlide,
   },
    setup(){
        const onSwiper = (swiper) => {
        // console.log(swiper);
      };
      const onSlideChange = () => {
        // console.log('slide change');
      };
      

      return{
        onSlideChange,
        modules: [Navigation, Pagination, Scrollbar, A11y , Autoplay , EffectFade],
        onSwiper,
      }
    }
}

</script>

<style lang="scss">
.mainteste{
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
   padding: 50px;
  width: 100%;
  margin-top: 50px;
  margin-bottom: 50px;
  background-color: rgb(184, 214, 226);
  h2{
   font-size: 50px;
  }
  .Testimonials{

  // padding: 150px 50px;
 width: 100%;
  display: flex;
  justify-content: center;
  // align-items: center;

  .boxx{
    width: 100%;
    display: flex;
    align-items: center;
    margin-bottom: 70px;
    gap: 30px;
       justify-content: center;
    .image{
         width: 50%;
      img{
        width: 100%;
        border-radius: 50%;
        border: 5px solid #fff;
      }

     
     
    }
    .text{
      width: 50%;
        display: flex;
        flex-direction: column;
        span{
          color: gray;
        }
        gap: 5px;
        p{
          font-size: 17px;
        }
      }
  }
}
}


</style>