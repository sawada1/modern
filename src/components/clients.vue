<template>
    <div>
        <div class="clients">
    <h2>our clients</h2>
    <div class=" images">
    <div class="image">
      <img src="../assets/img/clients/client-1.png" alt=""> 
    </div>
    <div class="image">
      <img src="../assets/img/clients/client-2.png" alt=""> 
    </div>
    <div class="image">
      <img src="../assets/img/clients/client-3.png" alt=""> 
    </div>
    <div class="image">
      <img src="../assets/img/clients/client-4.png" alt=""> 
    </div>
    <div class="image">
      <img src="../assets/img/clients/client-5.png" alt=""> 
    </div>
    <div class="image">
      <img src="../assets/img/clients/client-6.png" alt=""> 
    </div>
    <div class="image">
      <img src="../assets/img/clients/client-7.png" alt=""> 
    </div>
    <div class="image">
      <img src="../assets/img/clients/client-8.png" alt=""> 
    </div>
   
   
    </div>
   </div>
    </div>
</template>

<script setup>

</script>

<style lang="scss">
.clients{
    color: #fff;
  background-color: rgb(200, 232, 246);
  padding: 50px;
  margin-top: 50px;
  width: 100%;
//   height: 500px;
  h2{
    text-align: center;
    font-size: 40px;
    margin-bottom: 50px;
    color: #333;
  }
  .images{
    // padding: 50px;
    display: grid;
    grid-template-columns: repeat(4 , 1fr);
    background-color: #fff;
    // border: 2px solid #333;
    padding: 33px;
    width: 90%;
    // gap: 20px;
    margin: 10px 5%; 
    .image{
      border-right: 1px solid skyblue;
      padding: 20px;
      transform: scale(0.7);
      transition: 0.5s;
      &:hover{
        transform: scale(1);
      }
      img{
      width: 100%;
      height: 100%;
     
    }
    } 
    
  }
}


</style>