<template>
 
    <nav id="navbar">
       <div id="dalem">
        <h2>Nikkī</h2>
       
        <ul>
            <li><a href="#about">About</a></li>
            <li><a href="#skill-con">Skills</a></li>
            <li><a href="#projects">Projects</a></li>
            <li><a href="#contact">Contact</a></li>
         
        </ul>

    </div>
        
    </nav>
 
</template>

<script>

export default {
 
}
</script>

<style lang="scss" scoped>

#navbar{
    background: rgba(0, 0, 0, 0.2);
    backdrop-filter: blur(20px);
    padding: 0.4rem 0;
    width: 100%;
    position: fixed;
    top: 0;
    z-index: 100;
    font-size: 16px;
   
    
    #dalem{
       
        display: flex;
        width: 90%;
        margin: 0 auto;
        align-items: center;
        justify-content: space-between;
    }

        h2{
            font-weight: bold;
            font-size: 22px;
            cursor: pointer;
            display: block;
            background-image: linear-gradient(to right, #f464be, #df57cc, #c250dc, #9650ec, #4854fc);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }
    
 

    }

    ul{
        display: flex;
        
        
    
        li{
            margin: 0 8px;
            list-style-type: none;
            cursor: pointer;
            transition: color 10s;
            
            font-size: 1.1rem;
            padding: 1px 4px;

            a{
                
                text-decoration: none;
                color: #888c9c;
                transition: color 10s;
                transition: background-color 0.8s;
                border-radius: 5px;
              
                
            }
            
            a:hover{
               
                border-top: 2px solid #c250dc;
                border-bottom: 2px solid #c250dc;
                border-radius: 5px;
                
                

            }
            
            
        }

    
    }


@media (max-width: 640px){
    ul{
        li{
            a{
                font-size: 15px;
                padding: 3px;
            }
        }
    }

    #navbar{
        h2{
            font-size: 18px;
        }

    }
    
     
}

@media (max-width: 430px){
    ul{
        
        li{
            font-size: 10px;
           
        }
    }

    #navbar{
        h2{
            font-size: 16px;
        }

    }
    
     
}
</style>

