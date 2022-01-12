<template>
  <section>
    <div class="mobile_menu">
        <a href="#"><i class="ci-home_fill"></i></a>
        <a href="#"><i class="ci-search"></i></a>
        <a href="#"><i class="ci-message_circle"></i></a>
        <img src="../assets/logo.png" alt="">
    </div>
  </section>
</template>

<script>

</script>

<style>
    .mobile_menu{ 
        width: 240px;
        height: 4.7%;
        position: fixed;
        margin:auto;
        top: 90%;
        left:0;
        right:0;
        display: flex;
        justify-content: space-around;
        align-items: center;
        border-radius: 40px;
        background: #f5f5f5;
    }

    .mobile_menu > a {
        text-decoration: none;
        color: #000;
    }

    .mobile_menu > a > i {
        font-size: 1.2em;
    }

    .mobile_menu > img {
        width: 19px;
    }
</style>