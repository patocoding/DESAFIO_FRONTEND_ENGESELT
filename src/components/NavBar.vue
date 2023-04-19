<template>
   <header class="bg-slate-900 dark:bg-white">
    <nav class="p-4 text-gray-300 dark:text-gray-800 flex justify-between items-center w-[92%] mx-auto">
        <div>
            <h1 class="text-3xl font-[Poppins] font-semibold cursor-pointer" @click="router.push('/')">ZXY Tecnologia</h1>
        </div>
        <div class="nav-links changebg duration-500  md:static md:min-h-fit absolute min-h-[60vh] left-0 top-[-100%] md:w-auto w-full flex items-center p-5 rounded-lg z-50">
            <ul class=" flex md:flex-row flex-col md:items-center md:gap-[4vw] gap-8 font-[Poppins]">
                <li>
                    <a class="hover:text-gray-500 duration-300" href="#" @click="router.push('/Services')">Serviços</a>
                </li>
                <li>
                    <a class="hover:text-gray-500 duration-300" href="#" @click="router.push('/Clientes')">Clientes</a>
                </li>
          
                <li>
                    <a class="hover:text-gray-500 duration-300" href="#" @click="router.push('/Contato')">Contato</a>
                </li>
            </ul>
            
        </div>
            <div class="flex items-center gap-6">
            <!-- botão para ativar ou desativar modo noturno -->
               <dark-mode-button/>
               <ion-icon :name="iconName" @click="changeIconName" class="text-3xl cursor-pointer md:hidden"></ion-icon>
            </div>
           
        
    </nav>
   </header>
</template>

<script>
import DarkModeButton from '@/components/DarkModeButton.vue';
import '../assets/tailwind.css'
import { ref } from 'vue'
import { useRouter } from 'vue-router';

export default {
    name: 'NavBar',
    components :{
        DarkModeButton
    },
    setup () {
        const router = useRouter()
        const iconName = ref('menu');

        const changeIconName = (e) => {
            const navLinks = document.querySelector('.nav-links')
            const changebg = document.querySelector('.changebg')
            e.name = e.name === 'menu' ? 'close' : 'menu'
                // ação para abrir o menu
            navLinks.classList.toggle('top-[12%]')
            changebg.classList.toggle('bg-white')
           
        }
return {
    iconName,
    changeIconName,
    router
}

}
} 

</script>

<style scoped>
</style>


 

