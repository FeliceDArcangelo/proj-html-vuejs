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
            <div class="container">
                <div class="title">
                    <h2>Recent Work</h2>
                    <div>WEB - BRANDING - UX/UI</div>
                    <div class="bar"></div>
                </div>
                
            </div>
            <div class="portfolio-container">
                <div v-for="cards in store.cardsPortfolio" :key="cards.name">
                    <img  :src="cards.url">
                    <div class="card-name-after">{{ cards.message }}</div>
                </div>
            </div>
    </div>

    <button class="all-work-btn">VIEV ALL WORK</button>
</template>


<style lang="scss" scoped>
@use '../assets/styles/partials/variables' as *;

.pre-container{
    background-color: $my-first-green;
    .container{
    max-width: 1000px;
    margin: auto;
    padding-bottom: 6em;
    padding-top: 6em;
    color: $my-first-lille;
    .title{
        display: flex;
        flex-direction: column;
        align-items: center;
        h2{
            color: $my-first-white;
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
    .portfolio-container{
        display: flex;
        flex-wrap: wrap;
        div{
            width: 50%;
            aspect-ratio: 1/1;
            position: relative;
            img{
                object-fit: contain;
                height: 100%;
            }
            .card-name-after{
                position: absolute;
                top: 0;
                left: 0;
                background-color: $my-shadow-red;
                color: $my-first-white;
                font-size: large;
                width: 100%;
                text-align: center;
                padding-top: 50%;
                display: none;
            }
            &:hover .card-name-after{
                display: block;
                cursor: pointer;
            }
        }
    }
}
.all-work-btn{
    width: 100%;
    background-color: $my-first-red;
    border: none;
    height: 80px;
    color: $my-first-white;
    &:hover{
        cursor: pointer;
        color: $my-first-red;
        background-color: $my-first-white;
    }
}
</style>