<script>
    export default {
    
    }
</script>

<template>
  <div class="pre-container">
            <div class="container">
                <div class="title">
                    <h2>About Me</h2>
                    <div>UI & UX EXPERT</div>
                    <div class="bar"></div>
                </div>
                <div class="text">
                    <div>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Fuga quos iusto, voluptas, facilis dolorum esse, praesentium quae nostrum quod nulla debitis quam quasi dignissimos dolore quidem corporis voluptatem minima. Autem!
                    Minus, officia deleniti! Id, omnis nostrum tempore facere, libero fuga voluptatum, asperiores iusto adipisci assumenda ullam exercitationem dignissimos? Beatae, ratione sunt quos itaque dolore vel quibusdam doloremque omnis. Laudantium, incidunt!
                    Nesciunt repellendus animi optio aliquid, illum iste quas fuga fugiat voluptates quidem architecto enim corrupti perferendis minima? Molestiae fuga non, excepturi maxime similique dignissimos cumque saepe laborum atque repellendus dolorem.</div>
                    <div>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Enim, eos quos. Recusandae, illo maxime. Laudantium porro deserunt, repellat harum natus eum cum suscipit possimus! Sequi dolore vel illo quaerat magnam?
                    Architecto tempore praesentium minima, laborum eaque consequuntur. Alias ut dignissimos aut omnis voluptatem, similique placeat, corrupti perspiciatis ipsam modi neque voluptatibus debitis vel ipsum nesciunt laboriosam provident. Odit, dolore natus.
                    Nostrum, atque necessitatibus asperiores, expedita enim molestias, nihil voluptas ex blanditiis hic rem laboriosam esse inventore? Alias sint vero quia vel quas, laborum repellat autem eum? Vitae autem vero ducimus.</div>
                </div>
            </div>
        </div>
</template>


<style lang="scss" scoped>
@use '../assets/styles/partials/variables' as *;

.pre-container{
    background-color: $my-second-neavy;
    .container{
    max-width: 900px;
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
    }
    }
}
</style>