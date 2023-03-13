<template>
    <div>
        <div class="team" id="team">
     <h2>our team</h2>
     <div class="theimages">
      <img src="../assets/img/team-1.jpg" alt="">
     <img src="../assets/img/team-2.jpg" alt="">
     <img src="../assets/img/team-3.jpg" alt="">
     <img src="../assets/img/team-4.jpg" alt="">   
     </div>
  
   </div>
    </div>
</template>

<script setup>

</script>

<style lang="scss">
.team{
  padding: 30px;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  width: 100%;
  h2{
    text-align: center;
    font-size: 40px;
    margin-bottom: 50px;
  
  }
  .theimages{
    padding: 20px;
     display: grid;
     grid-template-columns: repeat(4 , 1fr);
    gap: 40px;
    img{
      width: 200px;
      border-radius: 50%;
      box-shadow: 10px 10px 10px rgba(0, 0, 0, 0.344);
    }
  }
}

</style>