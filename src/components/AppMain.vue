<script>
import store from '../store';
import Main1 from './Main1.vue'
import Main2 from './Main2.vue'
export default {
    data(){
        
        return{
            store,
        }
    },
    components: {
        Main1,
        Main2,
    }
}

</script>

<template>
    <main>
        <Main1/>
        <Main2/>
        <div class="portfolio-container">
            <img v-for="cards in store.cardsPortfolio" :key="cards.name" :src="cards.url">
        </div>
    </main>

</template>

<style lang="scss" scoped>
@use '../assets/styles/partials/variables' as *;

.portfolio-container{
    display: flex;
    flex-wrap: wrap;
    img{
        max-width: 50%;
        aspect-ratio: 1/1;
    }
}

</style>