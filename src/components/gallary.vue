<template>
    <div>
        
   <div class="portofolio">
    <h2>Our Portfolio</h2>
    <div class="allimages">
      <div class="theimage">
     <img src="../assets/img/portfolio/app1.jpg" alt="">
     <div class="back">
     <div class="text">
      <h3>app1</h3>
      <p>app description</p>
      <div class="icons">
        <i class="fa-solid fa-eye"></i>
        <i class="fa-solid fa-right-from-bracket"></i>
        </div>
     </div>
     </div>
     </div>
      <div class="theimage">
     <img src="../assets/img/portfolio/app2.jpg" alt="">
     <div class="back">
     <div class="text">
      <h3>app1</h3>
      <p>app description</p>
      <div class="icons">
        <i class="fa-solid fa-eye"></i>
        <i class="fa-solid fa-right-from-bracket"></i>
        </div>
     </div>
     </div>
     </div>
      <div class="theimage">
     <img src="../assets/img/portfolio/app3.jpg" alt="">
     <div class="back">
     <div class="text">
      <h3>app1</h3>
      <p>app description</p>
      <div class="icons">
        <i class="fa-solid fa-eye"></i>
        <i class="fa-solid fa-right-from-bracket"></i>
        </div>
     </div>
     </div>
     </div>
      <div class="theimage">
     <img src="../assets/img/portfolio/card1.jpg" alt="">
     <div class="back">
     <div class="text">
      <h3>app1</h3>
      <p>app description</p>
      <div class="icons">
        <i class="fa-solid fa-eye"></i>
        <i class="fa-solid fa-right-from-bracket"></i>
        </div>
     </div>
     </div>
     </div>
      <div class="theimage">
     <img src="../assets/img/portfolio/card2.jpg" alt="">
     <div class="back">
     <div class="text">
      <h3>app1</h3>
      <p>app description</p>
      <div class="icons">
        <i class="fa-solid fa-eye"></i>
        <i class="fa-solid fa-right-from-bracket"></i>
        </div>
     </div>
     </div>
     </div>
      <div class="theimage">
     <img src="../assets/img/portfolio/card3.jpg" alt="">
     <div class="back">
     <div class="text">
      <h3>app1</h3>
      <p>app description</p>
      <div class="icons">
        <i class="fa-solid fa-eye"></i>
        <i class="fa-solid fa-right-from-bracket"></i>
        </div>
     </div>
     </div>
     </div>
      <div class="theimage">
     <img src="../assets/img/portfolio/web1.jpg" alt="">
     <div class="back">
     <div class="text">
      <h3>app1</h3>
      <p>app description</p>
      <div class="icons">
        <i class="fa-solid fa-eye"></i>
        <i class="fa-solid fa-right-from-bracket"></i>
        </div>
     </div>
     </div>
     </div>
      <div class="theimage">
     <img src="../assets/img/portfolio/web2.jpg" alt="">
     <div class="back">
     <div class="text">
      <h3>app1</h3>
      <p>app description</p>
      <div class="icons">
        <i class="fa-solid fa-eye"></i>
        <i class="fa-solid fa-right-from-bracket"></i>
        </div>
     </div>
     </div>
     </div>
      <div class="theimage">
     <img src="../assets/img/portfolio/web3.jpg" alt="">
     <div class="back">
     <div class="text">
      <h3>app1</h3>
      <p>app description</p>
      <div class="icons">
        <i class="fa-solid fa-eye"></i>
        <i class="fa-solid fa-right-from-bracket"></i>
        </div>
     </div>
     </div>
     </div>
    </div>
   
   </div>
    </div>
</template>

<script setup>

</script>

<style lang="scss">
.portofolio{
  padding: 50px;
  .allimages{
    display: grid;
    grid-template-columns: repeat(3 , 1fr);
    gap: 20px;
    .theimage{
    width: 100%;
    height: fit-content;
    position: relative;
    border-radius: 30px;
    // overflow: hidden;
    img{
      width: 100%;
      border-radius: 30px;
    }
    .back{
      border-radius: 30px;
      position: absolute;
      top: 0%;
     
      width: 100%;
      height: 100%;
      background-color: rgba(0, 0, 255, 0.422);
      display: flex;
      justify-content: center;
      transition: 0.5s;
      opacity: 0;
     
      .text{
        color: #fff;
        display: flex;
        justify-content: center;
        align-items: center;
        flex-direction: column;
        h3{
        font-size: 35px;
      }
      p{
        font-size: 20px;
      }
        .icons{
          i{
            margin: 0px 20px;
            padding: 10px;
            font-size: 30px;
            background-color: var(--maincolor);
            cursor: pointer;
            border-radius: 10px;
         
          }
        }
      }
    }

   &:hover .back{
     opacity: 1;
   }
  }
  }
 
}

</style>