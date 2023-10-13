<template>
    <div id="skill-con">
        <h1>Skills & Tools</h1>
        <div class="skills">
            <div id="skill">
                <p>Languages</p>
                <div class="list">
                    <li>HTML</li>
                    <li>CSS</li>
                    <li>JavaScript</li>
                    <li>C</li>
                    <li>C++</li>
                    <li>Python</li>
                    <li>Java</li>

                </div>
            </div>

            <div id="skill">
                <p>FrontEnd</p>
                <div class="list">
                    <li>Vue.js</li>
                    <li>Vuex</li>
                    <li>React</li>
                    <li>Tailwind</li>
                </div>
            </div>

            <div id="skill">
                <p>BackEnd</p>
                <div class="list">
                    <li>ASP.NET</li>
                    <li>MySql</li>
                    <li>Golang</li>
                    <li>Laravel</li>
                </div>
            </div>

            <div id="skill">
                <p>Design</p>
                <div class="list">
                    <li>Figma</li>
                    <li>VisualParadigm</li>
                </div>
            </div>

        </div>
    </div>
</template>

<script>
import { Icon } from '@iconify/vue';
export default {
    components: {
		Icon,
	},
}
</script>

<style lang="scss">
#skill-con{
    
    padding-top: 15px;
    min-height: 100vh;
 

    h1{
        text-align: center;
        background-image: linear-gradient(to right, #4854fc, #9650ec, #c250dc, #df57cc, #f464be);
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;
        font-size: 80px;
       
    }



    #skill{
        margin: 20px 50px;
        border-radius: 5px;
     
       

        p{
            box-sizing: border-box;
            font-weight: bold;
            font-size: 20px;
            color: white;
            
            padding: 0 5px;
            display: inline;
        }


       .list{
        
        list-style-type: none;
        display: flex;
        align-items:center;
        flex-wrap: wrap;
       
        padding: 10px 5px;

        li{
            
            text-align: center; 
            background: #484554;
            margin: 3px 5px;
            width: fit-content;
            padding: 4.5px 8px;
            border-radius: 8px;
            cursor: pointer;
            color: #4854FC;
            font-weight: 500;
            font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
            
        }

       }
    }


}

@media (max-width: 960px) {
   #skill-con{
    h1{
        font-size: 80px;
    }
   }
}

@media (max-width: 640px) {
    #skill-con{
        h1{
            font-size: 60px;
        }
       }
}

</style>