<template>
    <button class="  py-2 px-4 rounded " @click="toggleDark()">
        <ion-icon name="flashlight" class="text-4xl  text-gray-500"></ion-icon>
    </button>
</template>

<script>
import { useDark, useToggle } from '@vueuse/core'
export default {
    
    setup(){
        const isDark = useDark()
        const toggleDark = useToggle(isDark)
  
        
        return {toggleDark, isDark}
    }
    

}


</script>

