<template>
    <div>
        <div class="services" id="services">
   <h2>services</h2>
   <div class="container mainbox">
    <div class="box">
      <i class="fa-solid fa-mobile-screen-button mobile"></i>
      <div class="text">
       <h3>Digital Marketing</h3>
       <p>Lorem ipsum dolor sit amet, consectetur 
       adipisicing elit. Aliquid dolorem laudantium deserunt 
       libero excepturi maiores accusamus placeat quisquam neque esse 
       iusto, enim possimus hic nisi laboriosam officiis asperiores reprehenderit ipsum.</p>
      </div>
    </div>
    <div class="box">
      <i class="fa-solid fa-globe world"></i>
      <div class="text">
       <h3>Branding</h3>
       <p>Lorem ipsum dolor sit amet, consectetur 
       adipisicing elit. Aliquid dolorem laudantium deserunt 
       libero excepturi maiores accusamus placeat quisquam neque esse 
       iusto, enim possimus hic nisi laboriosam officiis asperiores reprehenderit ipsum.</p>
      </div>
    </div>
    <div class="box">
      <i class="fa-regular fa-window-maximize web"></i>
      <div class="text">
       <h3>Web Design</h3>
       <p>Lorem ipsum dolor sit amet, consectetur 
       adipisicing elit. Aliquid dolorem laudantium deserunt 
       libero excepturi maiores accusamus placeat quisquam neque esse 
       iusto, enim possimus hic nisi laboriosam officiis asperiores reprehenderit ipsum.</p>
      </div>
    </div>
    <div class="box">
      <i class="fa-solid fa-camera camera"></i>
      <div class="text">
       <h3>Photo  &amp; Videography</h3>
       <p>Lorem ipsum dolor sit amet, consectetur 
       adipisicing elit. Aliquid dolorem laudantium deserunt 
       libero excepturi maiores accusamus placeat quisquam neque esse 
       iusto, enim possimus hic nisi laboriosam officiis asperiores reprehenderit ipsum.</p>
      </div>
    </div>
    <div class="box">
      <i class="fa-solid fa-pen-ruler design"></i>
      <div class="text">
       <h3>Creative Design</h3>
       <p>Lorem ipsum dolor sit amet, consectetur 
       adipisicing elit. Aliquid dolorem laudantium deserunt 
       libero excepturi maiores accusamus placeat quisquam neque esse 
       iusto, enim possimus hic nisi laboriosam officiis asperiores reprehenderit ipsum.</p>
      </div>
    </div>
    <div class="box">
      <i class="fa-solid fa-tablet-screen-button inter"></i>
      <div class="text">
       <h3>Interactive Solutions</h3>
       <p>Lorem ipsum dolor sit amet, consectetur 
       adipisicing elit. Aliquid dolorem laudantium deserunt 
       libero excepturi maiores accusamus placeat quisquam neque esse 
       iusto, enim possimus hic nisi laboriosam officiis asperiores reprehenderit ipsum.</p>
      </div>
    </div>
   </div>



   </div>
    </div>
</template>

<script setup>

</script>

<style lang="scss">
.services{
  padding: 10px;
  h2{
    font-size: 40px;
    text-align: center;
    margin: 50px 0px;
  }
  background-color: rgb(174, 216, 233);
  .mainbox{
    display: grid;
    grid-template-columns: repeat(2 , 1fr);
    gap: 20px;
    .box{
      display: flex;
      align-items: center;
      flex-direction: column;
      gap: 20px;
      background-color: #fff;
      border-radius: 30px;
      margin: 20px;
      box-shadow: 10px 10px 10px rgba(0, 0, 0, 0.45);
      padding: 20px;
      transition: 0.6s;
      .text{
        text-align: center;
      }
      &:hover{
        transform: translateY(10px);
      }
      i{
        font-size: 80px;
        &.mobile{
              color: tomato;
            }
            &.world{
              color: blue;
            }
            &.web{
              color: yellowgreen;
            }
            &.camera{
              color: skyblue;
            }
            &.design{
              color: orange;
            }
            &.inter{
              color: var(--maincolor);
            }
      }
    }
  }
}

</style>