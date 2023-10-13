<template>
 
    <nav id="navbar">
       <div id="logo">
        Nikkī
       </div>
        <ul>
           
            <li><a href="#about">About</a></li>
            <li><a href="#skill-con">Skills</a></li>
            <li><a href="#projects">Projects</a></li>
            <li><a href="#contact">Contact</a></li>
         
        </ul>
        
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
    padding: 10px 0;
    width: 100%;
    position: fixed;
    top: 0;
    z-index: 100;
    font-size: 16px;
    display: flex;
    justify-content: space-around;

    
    #logo{
        display: flex;
        align-items: center;
        background-image: linear-gradient(to right, #f464be, #df57cc, #c250dc, #9650ec, #4854fc);
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;
        font-weight: bold;
        font-size: 27px;
        width: 100px;
        justify-content: center;
        cursor: pointer;
    }
 

    }

    ul{
        display: flex;
        justify-content: flex-end;
        margin-right: 50px;
        align-content: center;
        
        
        li{
          
            display: block;
            cursor: pointer;
            margin: 0 15px;
            transition: color 10s;

           
            a{
                text-decoration: none;
                color: 
                    #888c9c;
                font-size: 1.1em;
                transition: color 10s;
                padding: 8px;
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
        #logo{
            font-size: 18px;
        }

    }
    
     
}
</style>

