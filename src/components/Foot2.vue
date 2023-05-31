<script>
import store from '../store'
    export default {
        data(){
            return{
                store,
            }
        }
    }
</script>

<template>
  <div class="pre-container">
    <div class="container">
        <img src="../assets/img/avada-footer-logo.png" alt="">
        <div class="copyrights">
            <div v-for="copy in store.arrCopyrights" :key="copy.id">
                {{ copy.name }}
                <span>{{ copy.fucus }}</span>
            </div>
        </div>
        <div class="social">
            <font-awesome-icon icon="fa-brands fa-twitter" />
        </div>
    </div>
  </div>
</template>


<style lang="scss" scoped>
@use '../assets/styles/partials/variables' as *;

.pre-container{
    background-color: $my-first-neavy;
    .container{
        max-width: 700px;
        margin: auto;
        text-align: center;
        .copyrights{
            display: flex;
            justify-content: center;
            gap: .5em;
            color: $my-first-lille;
            font-size: .8rem;
            span{
                color: $my-first-white;
            }
        }
        .social{
            color: white;
        }
    }
    
}

</style>