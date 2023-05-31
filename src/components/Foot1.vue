<script>

</script>

<template>
  <div class="pre-container">
            <div class="container">
                <div class="title">
                    <h2>Let's Work Together</h2>
                    <div>TELL ME MORE ABOUT YOUR PROJECT</div>
                    <div class="bar"></div>
                </div>
                <div class="text">
                    <div>Fuga quos iusto, praesentium quae nostrum quod nulla debitis quam quasi dignissimos dolore quidem corporis voluptatem minima. Autem!
                    Minus, officia deleniti! Id, omnis nostrum tempore facere, asperiores iusto adipisci assumenda ullam exercitationem dignissimos?</div>
                </div>
            </div>
            <form>
                <input type="text" name="" id="" placeholder="NAME">
                <input type="email" name="" id="" placeholder="EMAIL">
                <input type="number" name="" id="" placeholder="PHONE">
                <button>LET'S TALK</button>
            </form>
        </div>
</template>


<style lang="scss" scoped>
@use '../assets/styles/partials/variables' as *;

.pre-container{
    background-color: $my-second-white;
    .container{
    max-width: 1000px;
    margin: auto;
    padding-bottom: 6em;
    padding-top: 6em;
    color: $my-first-neavy;
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
            background-color: $my-first-neavy;
        }
    }
    .text{
        display: flex;
        gap: 2em;
        padding-top: 2em;
        text-align: center;
        max-width: 700px;
        margin: auto;
    }
    }
    form{
        display: flex;
        flex-direction: column;
        align-items: center;
        gap: .5em;
        padding-bottom: 6em;
        input, button{
            width: 400px;
            height: 50px;
            border: none;
            padding: 1em;
        }
        button{
            color: $my-first-white;
            background-color: $my-first-red;
        }
    }
}
</style>