<template>
   <header id="about">
       <navbar ref="navref"/>

       <div id="intro">
        <div id="text">

            <div id="intro-con">

                <p>
                    
                    <Icon class="animate__animated animate__tada animate__delay-2s animate__infinite tangan" icon="fxemoji:waving" width="40" height="40"  /> Hello, My Name is
                </p>
                <h1 id="Nicky"
                    class="animate__animated animate__fadeIn animate__delay-0.5s">Nicky Dharmawan
                </h1>
    
                <p id="myself">
                    i'm a Computer Science Student at Bina Nusantara University. I am deeply passionate about software development, particularly in Frontend, Backend also Fullstack Development.
                    i'm excited to use my knowledge and finding experience at your company. Thank you for visiting my portfolio!.
                    <br>
                    <br>
                   
                    Reach me out!!
                </p>
            </div>

            <div id="links">
                <a href="https://www.linkedin.com/in/nicky-dharmawan-971aa4290/" target="_blank">
                    <Icon class="animate__animated animate__slideInLeft animate__delay-0.5s" icon="mdi:linkedin" width="90" height="60" />
                </a>
                <a href="https://github.com/Nickyhehe?tab=repositories" target="_blank">
                    <Icon class="animate__animated animate__slideInUp animate__delay-0.5s" icon="mdi:github" width="90" height="60" />
                </a>
                <a  href="" target="_blank">
                    <Icon class="animate__animated animate__slideInRight animate__delay-0.5s" id="CV" icon="academicons:cv-square"  width="85" height="55" />
                </a>
                
            </div>
        </div>
      
       </div>
     

   </header>
    
  
  
</template>

<script>
import { Icon } from '@iconify/vue';
import navbar from './navbar.vue';
export default {
    components:{
        navbar,
        Icon,
    },

}
</script>

<style lang="scss">

header{

    min-height: 100vh;
    align-items: center;
 


    #intro{
      padding-top: 90px;
        text-align: center;
        
        
       
        #intro-con{
            
            width: 95%;
            margin: 0 auto;
            padding: 30px;

            #myself{
                font-size: 1.1em;
                display: block;
                text-align: center;
                margin: 0 auto;
                width: 80%;
                
            }
        }

        
    }
    
    p{
        font-size: 2em;
        color: white;
        font-weight: 600;
        display: inline;
    }
    h1{
        background: linear-gradient(to right, #30CFD0 0%, #330867 100%);
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;
        font-size: 5em;
        margin-top: -0.1em;
        
        
    }

    #links{
       
      
        a{
            text-decoration: none;
            transition: color 0.3s;
            color: white;
        }
        a:hover{
            color: #f464be;
        }

        #CV{
            margin-bottom: 3px;
        }
        
        
    }

    @media (max-width: 960px) {
       h1{
        font-size: 4em;
       }

       #intro{
        #intro-con{
    
            #myself{
                font-size: 1em;
               
            }
        }
       
        }
    }
    
    @media (max-width: 640px) {
    h1{
        font-size: 2.5em;
    }

    #intro{
        #intro-con{
            
            p{
                font-size: 1.6em;

                .tangan{
                    width: 40px;
                    height: 30px;
                }
            }
            #myself{
                font-size: 1em;
               
            }
        }
       
        }
    }


    
}

</style>