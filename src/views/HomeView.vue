<template>
  <div class="home">
   <landing/>
   <about/>

    <services/>
 

   <why/>
   
   <gallary/>

  <testi/>

  <team/>

  <clients/>

  <contact/>
 
 
  

 

   


   <div class="footer">
     <div class="linkss">
     <a href="#">home</a>
     <a href="#about">about us</a>
     <a href="#aboout">services</a>
     <a href="#aboout">team</a>
     <a href="#aboout">contact us</a>
     </div>
     <div class="logos">
      <i class="fa-brands fa-twitter"></i>
      <i class="fa-brands fa-facebook"></i>
      <i class="fa-brands fa-instagram"></i>
      <i class="fa-brands fa-youtube"></i>
     </div>
     <h3>2023 || created by <span>khaled sawada</span></h3>
     <div class="up" @click="upbtn">
    <i class="fa-solid fa-arrow-up"></i>
   </div>
   </div>

  </div>
</template>

<script>
// @ is an alias to /src
// import Swiper core and required modules

import {ref} from 'vue'



import landing from '../components/landing.vue'
import about from '../components/about.vue';
import services from '../components/services.vue';
import why from '../components/why.vue';
import gallary from '../components/gallary.vue';
import testi from '../components/testimon.vue';
import team from '../components/team.vue';
import clients from '../components/clients.vue';
import contact from '../components/contact.vue';


export default {
  name: 'HomeView',
  components: {
      landing,
      about,
      services,
      why,
      gallary,
      testi,
      team,
      clients,
      contact
  },
  setup(){



       let thecheck = ref(false)
       
     
      
       const upbtn = () =>{
        window.scrollTo({ top: 0, behavior: 'smooth' });
       }

    return{
   
     
      thecheck,
      upbtn,
    
    }
  }
}
</script>


<style lang="scss">
.home{
  position: relative;
  overflow-x: hidden;
}

h2{
  text-align: center;
}
















.footer{
  background-color: var(--maincolor);
  padding: 100px;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  position: relative;
  gap: 30px;
  .linkss{
    display: flex;
    align-items: center;
    gap: 30px;
    a{
      color: #fff;
      font-size: 15px;
    }
  }
  .logos{
    display: flex;
    align-items: center;
    gap: 20px;
    i{
      font-size: 30px;
      color: #fff;
    }
  }
  h3{
    color: #fff;
    font-size: 20px;
    text-align: center;
    span{
      color: tomato;
    }
  }
  .up{
  position: absolute;
  right: 50px;
  i{
    font-size: 20px;
    border-radius: 50%;
    color: #fff;
    cursor: pointer;
    border: 3px solid #fff;
    padding: 5px 10px;
    
  }
 
 
}
}


@media (max-width:587px){
  .footer{
    .linkss{
      flex-direction: column;
    }
    .logos{
      flex-direction: column;
    }
  }
}


@media(max-width:900px){
  .why{
    .themain{
      .boxes{
        grid-template-columns: repeat(2,1fr);     
      }
    }
  }
  .clients{
    padding: 0px;
    .images{
      padding: 0;
      grid-template-columns: repeat(2 , 1fr);
      img{
        margin: 20px 0px;
        width: 300px;
      }
    }
  }
}





@media(max-width:600px){
  .why{
    .themain{
      .boxes{
        grid-template-columns: repeat(1 , 1fr);
      }
    }
  }
}








@media(max-width:580px){
  .clients{
    // padding: 0px;
    // height: fit-content;
    margin-bottom: 50px;
    .images{
      // padding: 0;
      margin: 0;
      grid-template-columns: repeat(1 , 1fr);
      width: 100%;
      gap: 50px;
    }
  }
} 


@media(max-width:750px){
  .about{
    .maintext{
      width: 90%;
      flex-direction: column;
      .text1{
        width: 100%;
        gap: 50px;
        .ico{
        flex-direction: column;
        align-items: center;
        gap: 30px;
        }
       
        }
        .image{
          width:100%;
          img{
            width:100%;
          }
      }
    }
  }
  .services{
    .mainbox{
      grid-template-columns: repeat(1 , 1fr);
    }
  }
  .team{
    .theimages{
     grid-template-columns: repeat(2 , 1fr);
     img{
      width: 300px;
     }
    }
  }
}

@media (max-width:1100px){
  // .portofolio{
  //   .allimages{
  //     grid-template-columns: repeat(2 , 1fr);
  //   }
  // }
}
@media (max-width:770px){
  .portofolio{
    .allimages{
      grid-template-columns: repeat(1 , 1fr);
    }
  }

  .team{
    .theimages{
     grid-template-columns: repeat(1 , 1fr);
     img{
      width: 450px;
     }
    }
  }

}
@media (max-width:800px){
  .mainteste{
text-align: center;
width: 100%;
    .Testimonials{
       .boxx{
        flex-direction: column;
        width: 100%;
        
       .image{
        width: 100%;
       }
       .text{
        width: 100%;
        p{
          width: 100%;
        
        }
       }
       }
    }
  }
  .why{
    .themain{
      .numbers{
        flex-direction: column;
        gap: 30px;
      }
    }
  }
}

@media (max-width: 1033px){
   .landing{
    .image{
      img{
      width: 400px;
    }
    }
    // .maintext{
    //   h2{
    //     font-size: 40px;
    //   }
    
    // }
   
   }
}
  
  @media (max-width:820px){
    .landing{
      height: 700px;
      flex-direction: column;
      .image{
      img{
      width: 580px;
    }
    }
    // .maintext{
    //   h2{
    //     font-size: 50px;
    //   }
    
    // }
    }
  }


  @media(max-width:463px){
    .team{
      .theimages{
        img{
          width: 80%;
        }
      }
    }
  }
</style>
