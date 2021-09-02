<template>
    <div class="container">
        <div class="row">
        <TheBoxOne/>
        <TheBoxTwo/>
        <TheBoxThree/>
  

</div>
    </div>
</template>

<script>

import TheBoxOne from '@/components/TheBoxOne.vue'
 import TheBoxTwo from '@/components/TheBoxTwo.vue'
import TheBoxThree from '@/components/TheBoxThree.vue'


export default {
    name: "TheBoxes",
    components:{
        TheBoxOne,
       TheBoxTwo,
      TheBoxThree
    }
}
</script>