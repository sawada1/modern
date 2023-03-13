<template>
    <div>
        <div class="nav">
         <div class="logo">
            <!-- <h2>sawada</h2> -->
            <img src="../assets/img/logo.png" alt="">
         </div>
         <div class="mainlist" :class="{'active':check}">
            <div class="list">
                <div @click="toggle" class="close">
            <i  class="fa-solid fa-x"></i>
          </div>
          <ul>
          <li> <a href="#">home</a> </li>
          <li> <a href="#about">about</a> </li>
          <li> <a href="#services">services</a> </li>
          <li> <a href="#team">team</a> </li>
          <li> <a href="#contact">contact us</a> </li>
          </ul>
       
         </div>
        
         </div>
     
         <div @click="toggle" class="bar">
            <i class="fa-solid fa-bars"></i>
         </div>
        </div>
    </div>
</template>

<script>
import {ref} from 'vue';
export default {
    setup(){
        let check = ref(false);

        const toggle = ()=>{
            check.value = !check.value;
        }

        return{check , toggle}
    }
}
</script>

<style lang="scss">

   .nav{
    display: flex;
    align-items: center;
    box-shadow: 10px 10px 10px rgba(0, 0, 0, 0.403);
    padding: 25px;
    justify-content: space-between;
    position: fixed;
    z-index: 1111111111;
    left: 0;
    top: 0;
    right: 0;
    background-color: #fff;
    img{
        width: 150px;
        cursor: pointer;
    }
    .mainlist{
        // position: relative;
        .close{
            display: none;
        }
        .list{
        ul{
            display: flex;
            align-items: center;
            gap: 30px;
            li{
                margin: 0px 20px;
                a{
                    font-size: 20px;
                    color: #333;
                    transition: 0.5s;
                    &:hover{
                        color: var(--maincolor);
                        text-decoration: underline;
                    }
                }
            }
        }
    }
    }
   
    .bar{
        display: none;
        i{
            font-size: 35px;
            cursor: pointer;
            background-color: #ccc;
            padding: 10px;
            border-radius: 5px;
        }
    }
   }

   @media (max-width:1026px){
    .nav{
        .mainlist{
            .list{
            ul{
                gap: 10px;
                li{
                    margin: 0px 5px;
                }
            }
        }
        }
       
    }
   }
   @media (max-width:850px){
    .nav{
        position: relative;
        .bar{
            display: block;
        }
      .mainlist{
        top: 0%;
        left: 0;
        bottom: 0;
        width: 100vw;
        height: 100vh;
        background-color: rgba(0, 0, 0, 0.368);
        position: fixed;
        transform: translateX(200%);
        transition: 0.5s;
        &.active{
            transform: translateX(0);
        }
       
        .list{
            position: absolute;
            top: 0%;
            right: 0px;
            min-height: 100vh;
            width: 300px;
            z-index: 11111;
            background-color: #004a99;
            .close{
            display: block;
                position: absolute;
                font-size: 20px;
                margin-top: 20px;
                color: #fff;
                border: 3px solid #fff;
                padding: 10px 20px;
                border-radius: 50%;
                cursor: pointer;
                top: 0;
                left: 5%;
            }
            ul{
                margin-top: 30px;
                flex-direction: column;
                width: 100%;
                gap: 50px;
                justify-content: space-around;
                li{
                    a{
                        color: #fff;
                        &:hover{
                        color: #333;
                        text-decoration: underline;
                    }
                    }
                }
            }
        }
      }
    }
   }
</style>