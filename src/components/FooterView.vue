<template>
    <div class=" bg-slate-900 w-full ">
            <footer>
                <div class="z-30 flex flex-col ">
                    
                    <div class="flex items-center text-white text-center justify-center mt-4 mb-6">
                        <h1>ZXY Tecnologia <ion-icon name="planet"></ion-icon> <span class="font-Poppins">todos os direitos reservados</span></h1>                 
                    </div>
                    <div class="flex items-center text-white text-center justify-center mt-4">
                        <h1>Sobre</h1>                 
                    </div>
                    <div>
                        <p class=" text-white text-center text-sm font-Poppins">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,</p>
                    </div>
                    
                    <ul class="flex items-center justify-center flex-col text-white">
                        <li class="mb-4 mt-4 flex items-center">
                            <ion-icon name="logo-facebook" class="text-2xl"></ion-icon> <span class="text-lg font-Poppins">ZXY Tecnologia</span>
                        </li>
                        <li class="mb-4 flex items-center">
                            <ion-icon name="logo-twitter" class="text-3xl"></ion-icon> <span class="text-lg font-Poppins">@zxytecnlogia</span>
                        </li>                          
                        <li class='flex items-center'>
                            <ion-icon name="person" class="text-3xl"></ion-icon> <span class="text-lg font-Poppins cursor-pointer" @click="router.push('/Clientes')">Página de Clientes</span>
                        </li>

                    </ul>
                </div>
            </footer>
    </div>
</template>
<script>
import { useRouter } from 'vue-router';
export default {
    name: 'FooterView',
    setup(){

        const router = useRouter()
        return{router}
    }

    
}
</script>

