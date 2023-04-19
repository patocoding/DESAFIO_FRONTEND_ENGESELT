<template>
    <body class="bg-slate-800 h-full">
        <NavBar/>
        <div class="container w-full animation">
            <div class="text-3xl mt-10 font-bold font-[Poppins] mx-auto flex justify-center text-teal-100">
                Clientes
            </div>
            
            
            <div class="flex items-center justify-center min-h-screen mx-auto">
             
                <!-- grid dos serviços -->

                <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
                    <div class="text-3xl mt-10 font-bold font-[Poppins] mx-auto flex justify-center text-teal-100 items-center">
                <h1>Já solucionamos problemas para:</h1>
            </div>
                    <div class="rounded-xl shadow-lg">
                        <div class="p-5 flex flex-col bg-slate-700 rounded-xl">
                            <div class="rounded-xl overflow-hidden  p-5 shadow-lg">
                                <img :src="url" alt=""/>
                            </div>
                            <h5 class="text-2xl md:text-3xl font-medium mt-3 text-teal-100 font-Poppins">Cliente 1</h5>
                            <div class="flex items-start">
                                <p class="text-cyan-50 text-lg text-center mt-4 mb-4" >Nome</p>
                            </div>
                            
                            <p class="text-cyan-50 text-lg text-center font-bold
                            ">Cayo Bruno Alves</p>
                           
                        </div>
                    </div>
                    <div class="rounded-xl shadow-lg">
                        <div class="p-5 flex flex-col bg-slate-700 rounded-xl">
                            <div class="rounded-xl overflow-hidden  p-5 shadow-lg">
                                <img :src="url" alt=""/>
                            </div>
                            <h5 class="text-2xl md:text-3xl font-medium mt-3 text-teal-100 font-Poppins">Cliente 2</h5>
                            <div class="flex items-start">
                                <p class="text-cyan-50 text-lg text-center mt-4 mb-4" >Nome</p>
                            </div>                           
                            <p class="text-cyan-50 text-lg text-center font-bold
                            ">Verônica Alves</p>
                        </div>
                    </div>
                    </div>
                </div>
                
            </div>
            
    </body>
</template>

<script>
import NavBar from '@/components/NavBar.vue';
export default {
    components: {
        NavBar
    },
    setup(){
        return {

        }
    },
    data (){
        return{
            url: require('../assets/logo.png'),
            
        }
        
    }
}
</script>
<style scoped>
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