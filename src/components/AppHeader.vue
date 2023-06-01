<script>

</script>


<template>
  <header>
    <div class="title">
        <h4>AVADA FREELANCE</h4>
        <h1>Art Director</h1>
        <div>IF IT DOESN'T CHALLENGE YOU, IT DOESN'T CHANGE YOU</div>  
    </div>
    <div class="menu">
        <img src="../assets/img/av-freelance-logo-retina.png" alt="logo">
    </div>
    
  </header>
</template>


<style lang="scss" scoped>
@use '../assets/styles/partials/variables' as *;
    header{
        height: 100vh;
        background-image: url(../assets/img/banner_images.jpg); 
        object-fit: contain;
        position: relative;
        .title{
            height: 100%;
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
        .menu{
            position: absolute;
            top: 0;
            left: 0;
            height: 80px;
            width: 100%;
            padding-inline: 2em;
            padding: 1em;
            img{
                height: 80%;
            }
        }
    }
</style>