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
        <div class="text-slang">
            <img src="../assets/img/quotes-1.png" alt="quotes">
            <div class="famous-slang">"That's been one of my mantras - focus and simplicity. Simple can be harder than complex; you have to work hard to get your thinking clean to make it simple."</div>
            <div class="author-slang">STEVE JOBS - APPLE</div>
        </div>
        <div class="uni-brands">
            <div>TRUSTED MY GLOBAL BRANDS</div>
            <div class="uni-container" >
                <img v-for="uni in store.arrUniversities" :key="uni.name" :src="uni.url" alt="uni.name">
            </div>
        </div>
    </div>
  </div>
</template>


<style lang="scss" scoped>
@use '../assets/styles/partials/variables' as *;

.pre-container{
    background-image: url(../assets/img/testimonial_bkgd.jpg);

    .container{
        max-width: 900px;
        margin: auto;
        text-align: center;
        color: $my-first-white;
        .text-slang{
            img{
                margin: 3em;
                margin-top: 8em;
            }
            .famous-slang{
                font-style: italic;
            }
            .author-slang{
                margin: 2em;
                font-weight: bold;
            }
        }
        .uni-brands{
            padding: 3em;
            padding-top: 6em;
            .uni-container{
                display: flex;
                justify-content: center;
                gap: 8em;
                padding-top: 2em;
                img{
                    width: 50px;
                    aspect-ratio: 1/1;
                }
            }
        }
        
    }
}

</style>