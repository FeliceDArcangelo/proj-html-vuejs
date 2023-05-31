<script>
import store from '../store';
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
            <div class="container-title">
                <div class="title">
                    <h2>Expert Design Advice</h2>
                    <div>TRANDING DESIGN USE</div>
                    <div class="bar"></div>
                </div>
            </div>
            <div class="container-cards">
                <div class="card" v-for="news in store.arrDesignNews" :key="news.name">
                    <img :src="news.url" alt="">
                    <section>
                        <h2>{{ news.title }}</h2>
                        <p>{{ news.description }}</p> 
                    </section>
                    
                </div>

            </div>
    </div>
</template>


<style lang="scss" scoped>
@use '../assets/styles/partials/variables' as *;

.pre-container{
    background-color: $my-first-lille;
    .container-title{
    max-width: 1000px;
    margin: auto;
    padding-bottom: 6em;
    padding-top: 6em;
    color: $my-first-white;
    .title{
        display: flex;
        flex-direction: column;
        align-items: center;
        h2{
            font-size: 3rem;
        }
        div{
            margin: 1em;
        }
        .bar{
            width: 150px;
            height: 1.5px;
            background-color: $my-first-white;
        }
    }
    }
    .container-cards{
        display: flex;
        background-color: $my-first-neavy;
        .card{
            width: calc(100% / 3);
            img{
                width: 100%;
            }
            section{
                padding: 1em;
                padding-bottom: 2em;
                color: $my-first-lille;
                h2{
                    color: $my-first-red;
                }
            }
        }
    }
}
</style>