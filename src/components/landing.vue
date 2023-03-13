<template>
    <div>
        <div class="landing">
      <div class="maintext">
       <h2>we provide <span>solutions</span> for your business !</h2>
       <div class="btns">
        <button class="btn btn-primary">get started</button>
        <button class="btn btn-outline-primary">our services</button>
       </div>
      </div>
      <div class="image">
        <img src="../assets/img/intro-img.svg" alt="">
      </div>
    </div>
    </div>
</template>

<script setup>

</script>

<style lang="scss">

.landing{
  display: flex;
 padding: 50px;
 width: 100%;
 background-image: url('../assets/img/intro-bg.png');
background-size: cover;
 height: 660px;
 justify-content: space-around;
  align-items: center;
  // margin-top: 30px;
  margin-bottom: 50px; 
  gap: 70px;
  .image{
    img{
      width: 580px;
    }
  }
  .maintext{
    margin-top: 20px;
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 30px;
    h2{
      font-size: 30px;
      color: #fff;
      span{
        text-decoration: underline;
      }
    }
    .btns{
      display: flex;
      align-items: center;
      text-align: center;
      gap: 30px;
      button{
        padding: 10px 15px;
      }
    }
  }
}

</style>