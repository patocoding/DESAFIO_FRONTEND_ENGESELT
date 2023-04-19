<template>
    <body class="bg-slate-800 h-full ">
        <NavBar/>
        <div class="container w-full animation">
            <div class="text-3xl mt-10 font-bold font-[Poppins] mx-auto flex justify-center text-teal-100">Serviços</div>
            <div class="flex items-center justify-center min-h-screen mx-auto">
                <!-- grid dos serviços -->
                <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
                    <div class="rounded-xl shadow-lg">
                        <div class="p-5 flex flex-col items-center bg-slate-700 rounded-xl">
                            <div class="rounded-xl overflow-hidden bg-slate-100 p-5 shadow-lg">
                                <img :src="url" alt=""/>
                            </div>
                            <h5 class="text-2xl md:text-3xl font-medium mt-3 text-teal-100">Serviço 1</h5>
                            <p class="text-cyan-50 text-lg text-center
                            ">Lorem ipsum dolor sit amet consectetur adipiscing elit. Possimus expecu psoriaoas caravanis roniferous</p>
                            <button class="mt-4 bg-teal-500 text-white font-bold flex py-2 px-5 rounded-md items-center hover:bg-teal-700 duration-300" @click="router.push('/Clientes')">Clientes satisfeitos<ion-icon name="arrow-round-forward"></ion-icon></button>

                        </div>
                    </div>
                    <div class="rounded-xl shadow-lg">
                        <div class="p-5 flex flex-col items-center bg-slate-700 rounded-xl">
                            <div class="rounded-xl overflow-hidden bg-slate-100 p-5 shadow-lg">
                                <img :src="url" alt=""/>
                            </div>
                            <h5 class="text-2xl md:text-3xl font-medium mt-3 text-teal-100">Serviço 2</h5>
                            <p class="text-cyan-50 text-lg text-center
                            ">Lorem ipsum dolor sit amet consectetur adipiscing elit. Possimus expecu psoriaoas caravanis roniferous</p>
                            <button class="mt-4 bg-teal-500 text-white font-bold flex py-2 px-5 rounded-md items-center hover:bg-teal-700 duration-300" @click="router.push('/Clientes')">Clientes satisfeitos<ion-icon name="arrow-round-forward"></ion-icon></button>
                            
                        </div>
                    </div>
                    <div class="rounded-xl shadow-lg">
                        <div class="p-5 flex flex-col items-center bg-slate-700 rounded-xl">
                            <div class="rounded-xl overflow-hidden bg-slate-100 p-5 shadow-lg">
                                <img :src="url" alt=""/>
                            </div>
                            <h5 class="text-2xl md:text-3xl font-medium mt-3 text-teal-100">Serviço 3</h5>
                            <p class="text-cyan-50 text-lg text-center
                            ">Lorem ipsum dolor sit amet consectetur adipiscing elit. Possimus expecu psoriaoas caravanis roniferous</p>
                            <button class="mt-4 bg-teal-500 text-white font-bold flex py-2 px-5 rounded-md items-center hover:bg-teal-700 duration-300" @click="router.push('/Clientes')">Clientes satisfeitos<ion-icon name="arrow-round-forward"></ion-icon></button>
                            
                        </div>
                    </div>
                    
                </div>
                
            </div>
            <button class=" bg-teal-300 text-white font-bold flex py-2 px-5 rounded-md items-center hover:bg-teal-500 duration-300 " @click="router.push('/')">Home<ion-icon name="return-left"></ion-icon></button>
        </div>
    </body>
</template>

<script>

import NavBar from '@/components/NavBar.vue';
import { useRouter } from 'vue-router';

export default {
    components:{
        NavBar
    },
    setup() {
        // inicializando instancia do router
        const router = useRouter()
        return{ router }
    },
    data (){
        return{
            // necessário pois o vue não está pegando a imagem normalmente
            url: require('../assets/logo.png'),
            
        }
        
    }
}
</script>

<style scoped>


/* ANIMAÇÕES ABAIXO */
  .animation {
  animation-duration: 1.0s;
  animation-name: slidein;
}

  @keyframes slidein {
  from {
    opacity: 0.2;
    transform:translateY(-22%);
  }

  to {
    opacity: 1;
    transform:translateY(0%);
  }
}
</style>