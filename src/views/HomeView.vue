<template>
        <div id="home" class="bg-gray-800 dark:bg-gray-100 h-full">
            <NavBar />
            <div class="flex justify-center items-center mx-auto px-4 text-gray-200 mt-16">
                <h1 class="Bold text-3xl text-center font-[Poppins]">Bem-vindo(a) a</h1>
                
            </div>
            <div class="flex justify-center items-center mx-auto text-gray-200 mt-4">
                    <p class="bg-bookmark-white py-3 px-5 rounded-md text-bookmark-blue font-bold Bold text-3xl text-center font-[Poppins]">ZXY Tecnologia</p>
                </div>
            
            <section class="relative">
                <div class="container flex flex-col-reverse lg:flex-row items-center gap-12 mt-14 lg:mt-28">
        <!-- conteudo da pagina home -->
                    <div class="flex flex-1 flex-col items-center lg:items-start">
                    <h2 class="text-bookmark-white text-3xl md:text-4 lg:text-5xl text-center lg:text-left mb-6 font-Poppins tracking-wide mx-auto">
                        Nosso objetivo é 
                    </h2>
                    <p class="text-bookmark-purple font-bold pt-1 text-3xl md:text-4 lg:text-5xl text-center lg:text-left mb-6 font-Poppins tracking-wide mx-auto">EVOLUIR</p>
                    <p class="text-bookmark-grey text-md font-Roboto text-center lg:text-left mb-6">
                        Aqui na ZXY Tecnologia, fazemos de tudo para melhorar sua vida, evoluindo seu jeito de pensar e viver, fazendo isso da maneira mais natural possível. Conheça nossos serviços e Clientes
                    </p>
                    <div class="flex justify-center flex-wrap gap-6 mx-auto">
                        <button type="button" class="btn btn-purple white hover:bg-bookmark-white font-bold">
                        Serviços
                        </button>
                        <button type="button" class="btn btn-white hover:bg-bookmark-purple hover:text-white font-bold">
                        Clientes
                        </button>
                    </div>
                    </div>
                    <!-- Image -->
                    <div class="flex justify-center flex-1 mb-10 md:mb-16 lg:mb-0 z-10">
                    <img class="w-5/6 h-5/6 sm:w-3/4 sm:h-3/4 md:w-full md:h-full" :src="url" alt="" />
                    </div>
                </div>
                <!-- Rounded Rectangle -->
                <div
                    class="
                    hidden
                    md:block
                    overflow-hidden
                    bg-bookmark-purple
                    rounded-l-full
                    absolute
                    h-80
                    w-2/4
                    top-32
                    right-0
                    lg:
                    -bottom-28
                    lg:-right-36
                    "
                ></div>
        </section>
        <section class="bg-bookmark-white py-20 mt-20 lg:mt-60">
      <!-- Heading -->
      <div class="sm:w-3/4 lg:w-5/12 mx-auto px-2">
        <h1 class="text-3xl text-center text-bookmark-blue">Sobre a empresa</h1>
        <p class="text-center text-bookmark-grey mt-4">
         <b> A nossa empresa</b> é Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
        </p>
      </div>
      <!-- Feature #1 -->
      <div class="relative mt-20 lg:mt-24">
        <div class="container flex flex-col lg:flex-row items-center justify-center gap-x-24">
          <!-- Image -->
          <div class="flex flex-1 justify-center z-10 mb-10 lg:mb-0">
            <img
              class="w-5/6 h-5/6 sm:w-3/4 sm:h-3/4 md:w-full md:h-full"
              :src="url"
              alt=""
            />
          </div>
          <!-- Content -->
          <div class="flex flex-1 flex-col items-center lg:items-start">
            <h1 class="text-3xl text-bookmark-blue">Visão</h1>
            <p class="text-bookmark-grey my-4 text-center lg:text-left sm:w-3/4 lg:w-full">
                <b>Nossa visão</b> é Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
            </p>
          </div>
        </div>
        <!-- Rounded Rectangle -->
        <div
          class="
            hidden
            lg:block
            overflow-hidden
            bg-bookmark-purple
            rounded-r-full
            absolute
            h-80
            w-2/4
            -bottom-24
            -left-36
          "
        ></div>
      </div>
      <!-- Feature #2 -->
      <div class="relative mt-20 lg:mt-52">
        <div class="container flex flex-col lg:flex-row-reverse items-center justify-center gap-x-24">
          <!-- Image -->
          <div class="flex flex-1 justify-center z-10 mb-10 lg:mb-0">
            <img
              class="w-5/6 h-5/6 sm:w-3/4 sm:h-3/4 md:w-full md:h-full"
              :src="url"
              alt=""
            />
          </div>
          <!-- Content -->
          <div class="flex flex-1 flex-col items-center lg:items-start">
            <h1 class="text-3xl text-bookmark-blue">Missão e Valores</h1>
            <p class="text-bookmark-grey my-4 text-center lg:text-left sm:w-3/4 lg:w-full">
                <b>Nossas missões e valores são</b> Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
            </p>
          </div>
        </div>
        <!-- Rounded Rectangle -->
        <div
          class="
            hidden
            lg:block
            overflow-hidden
            bg-bookmark-purple
            rounded-l-full
            absolute
            h-80
            w-2/4
            -bottom-24
            -right-36
          "
        ></div>
      </div>
      <!-- Feature #3 -->
      <div class="relative mt-20 lg:mt-52">
        <div class="container flex flex-col lg:flex-row items-center justify-center gap-x-24">
          <!-- Image -->
          <div class="flex flex-1 justify-center z-10 mb-10 lg:mb-0">
            <img
              class="w-5/6 h-5/6 sm:w-3/4 sm:h-3/4 md:w-full md:h-full"
              :src="url"
              alt=""
            />
          </div>
          <!-- Content -->
          <div class="flex flex-1 flex-col items-center lg:items-start">
            <h1 class="text-3xl text-bookmark-blue">Breve Descrição dos serviços</h1>
            <p class="text-bookmark-grey my-4 text-center lg:text-left sm:w-3/4 lg:w-full">
              Nossos serviços são Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
            </p>
            <button type="button" @click="router.push('/Services')" class="btn btn-purple white hover:bg-bookmark-white">Serviços</button>
          </div>
        </div>
        <!-- Rounded Rectangle -->
        <div
          class="
            hidden
            lg:block
            overflow-hidden
            bg-bookmark-purple
            rounded-r-full
            absolute
            h-80
            w-2/4
            -bottom-24
            -left-36
          "
        ></div>
      </div>
    </section>
        </div>
        <FooterView/>
    
</template>

<script>
import NavBar from '@/components/NavBar.vue';
import FooterView from '@/components/FooterView.vue'
import '../assets/tailwind.css'
import { useRouter } from 'vue-router';


export default {
    components: {
        NavBar,
        FooterView
    },
    setup(){
        const router = useRouter()

        return { router }
    },
    data (){
        return{
            url: require('../assets/img/HomeImage.png'),
            
        }
        
    }
    
}


</script>

<style scoped>

.white{
    color: white;
}

.white:hover{
    color: black;
}
</style>