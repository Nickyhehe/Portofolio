<template>
  <div ref="contactref" class="contact-con" id="contact">
    <div id="text-con">
        <h1>Contact Me</h1>
    </div>
    <div id="infos"> 
        <a href="https://wa.me/6281297236948" target="_blank">
            <div id="wa">
                <h1>Whatsapp</h1>
                <p>+62 812-9723-6948</p>
            </div>
        </a>
        
        <a href="mailto:nickydharmawan1@gmail.com">
            <div id="gmail">
                <h1>Email</h1>
                <p>Nickydharmawan1@gmail.com</p>
            </div>
        </a>
    </div>

    <form >
        <div id="top">
            <div id="name">
                <label for="">Name</label>
                <input type="text" placeholder="Name" required>
            </div>

            <div id="email">
                <label for="">Email</label>
                <input type="email" placeholder="Email" required>
            </div>
            
        </div>
      
        <div id="msg">
            <label for="">Message</label>
            <textarea name="" id="" placeholder="Message"></textarea>
        </div>

        <div id="bottom">
            <p>Feel free to ask anything</p>
            <button>Send</button>
        </div>
       
    </form>
  </div>

</template>

<script>
export default {

}
</script>

<style lang="scss">

*{
    box-sizing: border-box;
}
.contact-con{

    min-height: 100vh;
    margin-top: 50px ;
    

    #infos{
        
        width: 70%;
        margin: 0 auto;
        display: flex;
        justify-content: space-between;
      
        flex-wrap: wrap;
        h1{
            font-size: 23px;
            
            margin: 0;
            
        }
        p{
           
            font-size: 18px ;
            margin: 0;
            color:#888c9c;
           
        }
        a{
            text-decoration: none;
            width: 48%;
            
            #wa, #gmail{
                background: #262626;
                padding: 15px 20px;
                border-radius: 10px;
                width: 100%;
                margin-bottom: 40px;
                cursor: pointer;
                color: white;
                transition: box-shadow 0.5s ease;
            }

        

        }

    }

    #wa:hover, #gmail:hover {
        box-shadow: 0px 1px 13px 1px rgba(194, 80, 220, 0.78);
        -webkit-box-shadow: 0px 1px 13px 1px rgba(194, 80, 220, 0.78);
        -moz-box-shadow: 0px 1px 13px 1px rgba(194, 80, 220, 0.78);
    }
   
    #text-con{
        background-image: linear-gradient(to left, #4854fc, #9650ec, #c250dc, #df57cc, #f464be);
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;
        text-align: center;
        box-sizing: border-box;
        font-size: 30px;
        padding: 20px 0;
    }
    form{
        border: transparent solid 0.1px;
        background: #262626;
        width: 70%;
        margin: 0 auto;
        padding: 20px;
        box-sizing: border-box;
        color: white;
        border-radius: 10px;
        font-size: 16px;
        transition: box-shadow 0.5s ease;

        label{
            display: block;
            margin-bottom: 7px;
        }

        input{
            width: 100%;
            border-radius: 5px;
            background-color: transparent;
            box-shadow: none;
            outline: none;
            border: 1px solid white;
            color: white;
            padding: 8px;
            height: 40px;
        }

        input::placeholder{
            font-size: 14px;
    
        }
        #top{
           margin: 20px 0;
            #name, #email{
                display: inline-block;
                width: 45%;

            
            }

            #email{
                float: right;
            }
            
            
        }

        #msg{

            textarea{
                width: 100%;
                height: 100px;
                border-radius: 5px;
                background-color: transparent;
                box-shadow: none;
                outline: none;
                border: 1px solid white;
                color: white;
                padding: 8px;
            }
        }

    }

    form:hover{
        box-shadow: 0px 1px 13px 1px rgba(194,80,220,0.78);
-webkit-box-shadow: 0px 1px 13px 1px rgba(194,80,220,0.78);
-moz-box-shadow: 0px 1px 13px 1px rgba(194,80,220,0.78);
    }

    #bottom{
     
        margin: 20px auto 0 auto;
       

        p{
            display: inline-block;
         
        }
        button{
           float: right;
           color: white;
           background: #4854fc;
           border-radius: 10px;
           padding: 2.5vh 6vw;
           cursor: pointer;
           font-weight: bold;
           font-size: 1.1em;
           border: none;
         
           
           
        }
     

      
    }


}

@media (max-width: 960px) {
    .contact-con form{
       
        width: 80%;
        
    }

    .contact-con{
        #infos{
           width: 80%;

           a{
            width: 100%;
           }
          
        }
    }
}
@media (max-width: 640px){
    .contact-con form{
       
        width: 90%;
        
    }

    .contact-con{
        #infos{
           width: 90%;

        
        }
    }
}

</style>