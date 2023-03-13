<template>
    <div>
        <div class=" about" id="about">
    <h2>about us</h2>
    <div class="maintext">
       <div class="text1">
         <p>Lorem ipsum, dolor sit amet
          consectetur adipisicing elit. 
          Neque eum voluptatum natus eveniet illo corporis voluptates animi, vel suscipit cumque,
          ducimus omnis expedita. Quis earum perspiciatis deleniti minus voluptates. Eaque.</p>
          <div class="ico">
            <i class="fa-solid fa-volume-high"></i>
             <div class="textt">
              <h4>title #1</h4>
              <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Expedita, porro?</p>
             </div>
          </div>
          <div class="ico">
            <i class="fa-solid fa-scale-balanced"></i>
             <div class="textt">
              <h4>title #2</h4>
              <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Expedita, porro?</p>
             </div>
          </div>
          <div class="ico">
            <i class="fa-solid fa-globe"></i>
             <div class="textt">
              <h4>title #3</h4>
              <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Expedita, porro?</p>
             </div>
          </div>
       </div>
       <div class="image">
        <img src="../assets/img/about-img.svg" alt="">
       </div>
    </div>
    <div class="maintext">
      <div class="image">
        <img src="../assets/img/about-extra-1.svg" alt="">
       </div>
       <div class="text1">
       <h3>About us secondary content title</h3>
         <p>Lorem ipsum, dolor sit amet
          consectetur adipisicing elit. 
          Neque eum voluptatum natus eveniet illo corporis voluptates animi, vel suscipit cumque,
          ducimus omnis expedita. Quis earum perspiciatis deleniti minus voluptates. Eaque.</p>
       </div>
     
    </div>
    <div class="maintext">
       <div class="text1">
       <h3>About us secondary content title</h3>
         <p>Lorem ipsum, dolor sit amet
          consectetur adipisicing elit. 
          Neque eum voluptatum natus eveniet illo corporis voluptates animi, vel suscipit cumque,
          ducimus omnis expedita. Quis earum perspiciatis deleniti minus voluptates. Eaque.</p>
       </div>
       <div class="image">
        <img src="../assets/img/about-extra-2.svg" alt="">
       </div>
    </div>
   </div>
    </div>
</template>

<script setup>

</script>

<style lang="scss">
.about{
  // margin: 60px 0px;
  width: 100%;
  h2{
    text-align: center;
    font-size: 40px;
    margin-bottom: 50px;
  }
  .maintext{
    width: 90%;
    margin-left: 5%;
    margin-right: 5%;
    display: flex;
    align-items: center;
    gap: 20px;
    margin-bottom: 100px;
    p{
      font-size: 18px;
    }
    .text1{
     width: 50%;
     .ico{
      display: flex;
      align-items: center;
      gap: 30px;
      i{
        font-size: 30px;
        border: 2px solid var(--maincolor);
        border-radius: 50%;
        padding: 10px;
        color: var(--maincolor);
        cursor: pointer;
        transition: 0.6s;
        &:hover{
          background-color: var(--maincolor);
          color: #fff;
        }

      }
      p{
        color: #3333339c;
      }
     }
    }
    .image{
      width: 50%;
      img{
        width: 100%;
      }
    }
  }
}

</style>