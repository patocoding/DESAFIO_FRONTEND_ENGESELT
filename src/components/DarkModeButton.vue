<template>
        <button class="flex  py-2 px-4 rounded items-center duration-300" @click="toggleDark()">
        <ion-icon name="flashlight" class="text-4xl  text-gray-500"></ion-icon> Modo {{isDark ? 'Escuro' : 'Claro'}} <!-- mudando o nome se estiver claro ou escuro -->
    </button>
    
</template>

<script>
import { useDark, useToggle } from '@vueuse/core'
export default {
    
    setup(){

        //funções dedicas a trocar o valor do DarkMode
        const isDark = useDark()
        const toggleDark = useToggle(isDark)
  
        
        return {toggleDark, isDark}
    }
    

}


</script>

