<template>
  <main>
    <div ref="projects" id="projects">

        <div id="pro-text">
            <h1>My Projects</h1>
            <p>Here is some of my projects.</p>
        </div>
        
        <div id="pro-con">

            <div v-for="project in projects" :key="project.id">
                <div id="project">

                    <div id="isinya" >
                        <img :src="project.image" :alt="project.image">
        
                        <div id="desc">
                            <h1>{{project.name}}</h1>
                            <p>{{project.desc}}</p>
                         </div>
                         
                    <div id="buttons">
                       
                        <p>
                            <a :href="project.linkCode" target="_blank">
                                <Icon class="icon" icon="entypo-social:github" width="25" />
                                Code
                            </a>
                        </p>
                        <p>
                            <a :href="project.links" target="_blank">
                                <Icon class="icon" icon="ion:open-outline" width="25" />
                                Live View
                            </a>
                        </p>
                    </div>
                    
                
                    </div>
                    
                </div>
            </div>

           

        </div>

    </div>
  </main>
  
</template>

<script>
import Nukang from '../assets/Nukang.png'
import ComingSoon from '../assets/gerak1.gif'
import Porto from '../assets/Porto.png'
import UTS from '../assets/UTS.png'
import { Icon } from '@iconify/vue';
export default {
    components: {
		Icon,
	},

    data(){
        return{
            projects: [
                {
                id: 1,
                name: 'Nukang.Com',
                desc: "Nukang.Com is a part of Binus University Project, offering a convenient online platfrom to find reliable handyman services. Built using ASP.NET, HTML , CSS and SQL Server",
                image: Nukang,
                links: "https://github.com/Nickyhehe/Nukangs.COM",
                linkCode: "https://github.com/Nickyhehe/Nukangs.COM",

            },
            {
                id: 2,
                name: 'Portfolio',
                desc: 'My own portfolio website as a showcase and a portfolio. This application was also related to binus intership program, becase it required a website. I built this website with Vue,js, Vuex',
                image: Porto,
                links: "https://portofolio-one-gules.vercel.app/",
                linkCode: "https://github.com/Nickyhehe/Portofolio"

            },
            {
                id: 3,
                name: 'UnderTheSea',
                desc: 'This website is a project task assigned by Binus in the subject HCI. This webiste is about the information of life under the sea. This project is created with pure Vanilla HTML, CSS, and Javascript',
                image: UTS,
                links: "https://under-the-sea-three.vercel.app/",
                linkCode: "https://github.com/Nickyhehe/UnderTheSea"

            },
            {
                id: 4,
                name: 'Coming Soon',
                desc: 'test',
                image: ComingSoon,

            },
            {
                id: 5,
                name: 'Coming Soon',
                desc: 'test',
                image: ComingSoon,

            },
            {
                id: 6,
                name: 'Coming Soon',
                desc: 'test',
                image: ComingSoon,
                    
            },

            ]
        }
    },
    
 

}
</script>

<style lang="scss">

main{
  
}

#pro-text{
    text-align: center;
    color: white;
    padding: 1px 0;
    h1{
        font-size: 100px;
        background: #4854FC;
        background: linear-gradient(to right, #4854FC 0%, #51D0A1 100%);
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;
    }
    p{
        font-size: 1.5rem;
    }

}



#pro-con{
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(calc(33.333% - 40px), 1fr));
  
    padding: 0 30px;
    

    #project{
        
        border: transparent solid 0.1px;
        margin: 25px 30px;
        color: white;
        border-radius: 10px;
        box-sizing: border-box;
        -webkit-box-shadow: 0px 0px 22px -2px rgba(72,84,252,1);
        -moz-box-shadow: 0px 0px 22px -2px rgba(72,84,252,1);
        box-shadow: 0px 0px 22px -2px rgba(72,84,252,1);
       
        #isinya{
           
           
            margin: 18px;
         
            #desc{
                margin-top: -10px;
                overflow: hidden;
                height: 177px;
               

                h1{
                    font-size: 21px;
                    background: linear-gradient(to right, #4854FC 0%, #30CFD0 100%);
                    -webkit-background-clip: text;
                    -webkit-text-fill-color: transparent;
                        }
                p{
                    
                    margin-top:-10px ;
                    color: 
                    #888c9c;
                }
            }

         
            img{
                width: 100%;
                height: 180px;
                border-radius: 10px;
                
            }
            #buttons{
                display: flex;
                justify-content: space-between;
                p{
                    display: flex;
                    justify-content: space-between;

                    cursor: pointer;
                    width: 48%;
                    background: #4854fc;
                    text-align: center;
                    padding: 10px 0;
                    border-radius: 6px;
                    margin: 0;
                    font-weight: bold;
                    transition: background-color 0.3s;
                    justify-content: center;
                    align-items: center;

                    .icon{
                        vertical-align: bottom;
                        margin-right: 5px;
                    }
                }
                p:hover{
                    background-color: #1B9AD0;
                }
                p:last-child{
                    float: right;
                }
                a{
                    color: white;
                    text-decoration: none;
                      
                }
            }
            
        }

    
    }
}

@media (max-width: 960px) {
    #pro-con {
        grid-template-columns: repeat(auto-fill, minmax(calc(50% - 40px), 1fr));
    }

    #pro-text{
        h1{
            font-size: 85px;
        }
    }
}

@media (max-width: 640px) {
    #pro-con {
        grid-template-columns: repeat(auto-fill, minmax(calc(100% - 40px), 1fr));
        padding: 0 10px;
    }

    #pro-text{
        h1{
            font-size: 70px;
        }
    }
}



</style>