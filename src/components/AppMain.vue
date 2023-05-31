<script>
import store from '../store';
import Main1 from './Main1.vue'
import Main2 from './Main2.vue'
import Main3 from './Main3.vue'
import Main4 from './Main4.vue'
import Main5 from './Main5.vue'
export default {
    data(){
        return{
            store,
        }
    },
    components: {
        Main1,
        Main2,
        Main3,
        Main4,
        Main5,
    }
}

</script>

<template>
    <main>
        <Main1/>
        <Main2/>
        <Main3/>
        <Main4/>
        <Main5/>
    </main>

</template>

<style lang="scss" scoped>
@use '../assets/styles/partials/variables' as *;



</style>