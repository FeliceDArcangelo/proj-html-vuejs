<script>
    export default {
    
    }
</script>

<template>
  <div class="pre-container">
            <div class="container">
                <div class="title">
                    <h2>Why Work With Me</h2>
                    <div>WEB - BRANDING - UI/UX</div>
                    <div class="bar"></div>
                </div>
                <div class="text">
                    <div>Fuga quos iusto, praesentium quae nostrum quod nulla debitis quam quasi dignissimos dolore quidem corporis voluptatem minima. Autem!
                    Minus, officia deleniti! Id, omnis nostrum tempore facere, asperiores iusto adipisci assumenda ullam exercitationem dignissimos?</div>
                </div>
            </div>
            <font-awesome-icon :icon="['fas', 'user']" />
        </div>
</template>


<style lang="scss" scoped>
@use '../assets/styles/partials/variables' as *;

.pre-container{
    background-color: $my-first-neavy;
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
    .text{
        display: flex;
        gap: 2em;
        margin-top: 2em;
        text-align: center;
        max-width: 700px;
        margin: auto;
    }
    }
}
</style>