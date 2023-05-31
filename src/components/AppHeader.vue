<script>

</script>


<template>
  <header>
    <h4>AVADA FREELANCE</h4>
    <h1>Art Director</h1>
    <div>IF IT DOESN'T CHALLENGE YOU, IT DOESN'T CHANGE YOU</div>
  </header>
</template>


<style lang="scss" scoped>
@use '../assets/styles/partials/variables' as *;
    header{
        height: 100vh;
        background-image: url(../assets/img/banner_images.jpg); 
        object-fit: contain;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        h4{
            color: $my-first-white;
            font-size: 1.5rem;
        }
        h1{
            color: $my-first-red;
            font-size: 8rem;
        }
        div{
            color: $my-first-lille;
        }
    }
</style>