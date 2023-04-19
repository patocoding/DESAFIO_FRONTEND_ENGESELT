<template>
    <div>
        <NavBar/>
    </div>
    <body class=" container antialised bg-slate-800 animation">
        <div class="flex w-full min-h-screen justify-center items-center">
            <div class="flex flex-col space-y-6 bg-cyan-700 w-full max-w-4xl p-8 rounded-xl shadow-lg">
                <!-- área de informaçoes -->
                <div class="flex flex-col space-y-8 justify-between ">
                    <div>
                        <h1 class="font-bold text-4xl tracking-wide font-Poppins text-white">Contate-nos</h1>
                        <p class="pt-2 text-cyan-100 text-sm">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. </p>
                    </div>
                    <div class="flex flex-col space-y-6">
                        <div class="inline-flex space-x-2 items-center">
                            <ion-icon name="call" class="text-teal-300 text-xl"></ion-icon>
                            <span class="text-teal-300 ">(12) 3456-7890</span>
                        </div>
                        <div class="inline-flex space-x-2 items-center">
                            <ion-icon name="mail" class="text-teal-300 text-xl"></ion-icon>
                            <span class="text-teal-300 ">zxytecnlogia@gmail.com</span>
                        </div>
                        <div class="inline-flex space-x-2 items-center">
                            <ion-icon name="pin" class="text-teal-300 text-xl"></ion-icon>
                            <span class="text-teal-300 ">Rua Francisco Carneiro de Araújo, 55, Cabo Branco.</span>
                        </div>
                    </div>
                    <div class="flex space-x-4 text-lg">
                        <a href=""><ion-icon class="text-white" name="logo-facebook"></ion-icon></a>
                        <a href=""><ion-icon class="text-white" name="logo-twitter"></ion-icon></a>
                        <a href=""><ion-icon class="text-white" name="logo-instagram"></ion-icon></a>
                    </div>
                </div>
                <div class="bg-white rounded-xl shadow-lg p-8">
                    <!-- formulário de inscrição -->
                    <form class="flex flex-col space-y-4">
                        <div>
                            <label for="" class="text-sm text-gray-600">Nome completo</label>
                            <input type="text" placeholder="Seu nome completo" class="ring-1 ring-gray-300 w-full rounded-md px-4 py-2 outline-none focus:ring-2 focus:ring-teal-300"/>
                        </div>
                            <div>
                                <label for="" class="text-sm text-gray-600">E-mail</label>
                                <input type="text" placeholder="Seu melhor e-mail" class="ring-1 ring-gray-300 w-full rounded-md px-4 py-2 outline-none focus:ring-2 focus:ring-teal-300"/>
                            </div>
                            <div>
                                <label for="" class="text-sm text-gray-600">Mensagem</label>
                                <textarea type="text" placeholder="Mensagem..." class="ring-1 ring-gray-300 w-full rounded-md px-4 py-2 outline-none focus:ring-2 focus:ring-teal-300"/>
                            </div>
                            <button class="inline-block self-end bg-cyan-700 text-white font-bold rounded-lg px-6 py-2 uppercase text-sm">ENVIAR MENSAGEM</button>
                    </form>
                </div>
            </div>
        </div>
    </body>
</template>

<script>
import NavBar from '@/components/NavBar.vue';
export default {
    
    components:{
        NavBar
    },
    setup() {
        return{ }
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
