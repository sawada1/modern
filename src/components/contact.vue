<template>
    <div>
        
   <div class="contact" id="contact">
   <h2>contact us</h2>
   <p>Want to work with us on a future project? Fill out the form below to get started!</p>
   <form action="" @click.prevent>
   <div class="inp">
   <input type="text" placeholder="your name">
   <input type="email" placeholder="your email">
   </div>
   <input type="text" placeholder="subjet">
   <textarea style="resize:none;" name="" id="" cols="30" rows="10" placeholder="message"></textarea>
   <button class="btn btn-primary">send message</button>
   </form>
   </div>

    </div>
</template>

<script setup>

</script>

<style lang="scss">
.contact{
  padding: 60px;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  width: 100%;
  gap: 30px;
  form{
    // width: 100%;
    display: flex;
    flex-direction: column;
    gap: 30px;
  }
  input,textarea{
    padding: 10px;
    outline: none;
    // width: 50%;
    margin: 10px 10px;
    border-radius: 20px;
  }
  button{
    // width: 30%;
    text-align: center;
  }
}


</style>