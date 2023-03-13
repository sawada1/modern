<template>
    <div>
        <div class="why">
     <div class="themain">
      <h2>Why choose us?</h2>
       <div class="boxes">
          <div class="box">
            <i class="fa-solid fa-pen"></i>
             <h3>Design Forward</h3>
             <p>Lorem ipsum dolor sit amet 
             consectetur adipisicing elit.
              Magni tempora laborum fugit corporis sequi, magnam odio laboriosam ad voluptatum 
             nesciunt optio, repellat, facere delectus mollitia rerum vel. Id, sequi rerum!</p>
             <span>read more</span>
          </div>
          <div class="box">
            <i class="fa-solid fa-pen"></i>
             <h3>Design Forward</h3>
             <p>Lorem ipsum dolor sit amet 
             consectetur adipisicing elit.
              Magni tempora laborum fugit corporis sequi, magnam odio laboriosam ad voluptatum 
             nesciunt optio, repellat, facere delectus mollitia rerum vel. Id, sequi rerum!</p>
             <span>read more</span>
          </div>
          <div class="box">
            <i class="fa-solid fa-pen"></i>
             <h3>Design Forward</h3>
             <p>Lorem ipsum dolor sit amet 
             consectetur adipisicing elit.
              Magni tempora laborum fugit corporis sequi, magnam odio laboriosam ad voluptatum 
             nesciunt optio, repellat, facere delectus mollitia rerum vel. Id, sequi rerum!</p>
             <span>read more</span>
          </div>
       </div>
       <div class="numbers">
        <div class="num">
         <span class="thenum">{{ num1 }}</span>
         <span>clients</span>
        </div>
        <div class="num">
         <span class="thenum">{{ num2 }}</span>
         <span>project</span>
        </div>
        <div class="num">
         <span class="thenum">{{ num3 }}</span>
         <span>Hours of Support</span>
        </div>
        <div class="num">
         <span class="thenum">{{ num4 }}</span>
         <span>Hours of Support</span>
        </div>
       </div>
     </div>
   </div>
    </div>
</template>

<script>


import {ref} from 'vue'
export default {
  
    setup(){
        let num1 = ref(0);
       let num2 = ref(0);
       let num3 = ref(0);
       let num4 = ref(0);

        const counter = ()=>{
            let section = document.querySelector('.numbers');
                      window.onscroll = ()=>{
                if(window.scrollY >= 3700){
                        let thecount1 = setInterval(() => {
                           if(num1.value == 300){
                             clearInterval(thecount1);
                           } else{
                            num1.value += 1
                           }
                          
                        }, 10 / 300);
                        let thecount2 = setInterval(() => {
                           if(num2.value == 450){
                             clearInterval(thecount2);
                           } else{
                            num2.value += 1
                           }
                          
                        }, 10 / 450);
                        let thecount3 = setInterval(() => {
                           if(num3.value == 1500){
                             clearInterval(thecount3);
                           } else{
                            num3.value += 1
                           }
                          
                        }, 1);
                        let thecount4 = setInterval(() => {
                           if(num4.value == 790){
                             clearInterval(thecount4);
                           } else{
                            num4.value += 1
                           }
                          
                        }, 10 / 790);
              } 

        }
        
       }
      
    
       counter();

       return{num1 , num2 , num3 , num4}
    }
    
}

</script>

<style lang="scss">

.why{
  margin-bottom: 80px;
  padding: 20px;
  background-color: var(--maincolor);
  width: 100%;
  h2{
    font-size: 40px;
    margin: 50px 0px;
    color: #fff;
  }
  .themain{
    display: flex;
    flex-direction: column;
    align-items: center;
    width: 100%;
    .boxes{
      display: grid;
      align-items: center;
      grid-template-columns: repeat(3 , 1fr);
      // gap: 10px;
      width: 100%;
     .box{
      display: flex;
      flex-direction: column;
      align-items: center;
      gap: 20px;
      background-color: #33333329;
      color: #fff;
      margin: 20px;
      padding: 60px 30px;
      border-radius: 20px;
      transition: 0.6s;
      cursor: pointer;
      span{
        margin-top: 30px;
        transition: 0.6s;
      }
      i{
        font-size: 50px;
      }
      &:hover{
        background-color: #3333335e;
      }
      &:hover span{
        text-decoration: underline;
      }
     }
    }
    .numbers{
      margin-top: 50px;
      display: flex;
      justify-content: space-around;
      width: 100%;
      color: #fff;
      .num{
       display: flex;
       flex-direction: column;
       align-items: center;
       gap: 5px;
       span{
        font-size: 20px;
       }
       .thenum{
        font-size: 55px;
        font-weight: bold;
       }
      }
    }
  }
}


</style>