<template>
  <section>
    <div class="object_menu">
      <div class="menu_under">
        <div class="object_plus"><span>+</span></div>
        <div class="object_quest"><span>?</span></div>
      </div>
    </div>
  </section>
</template>

<style>
  .obert {
    height: auto;
    padding: 10px 20px 10px 15px;
    text-align: center;
    margin: 0px auto 0px 279px;
  }

  .menu_under {
    position: fixed;
    top: 85%;
    left: 93.5%;
  }

  .object_plus, .object_quest{
    width: 2.1vw;
    height: 2.1vw;
    margin: 10px;
    display: flex;
    align-items: center;
    justify-content: center;
    background: #fff;
    border-radius: 40px;
    font-weight: bold;
    font-size: 1.4vw;
    color: #000;
  }

  .object_plus {
    font-size: 2.1vw;
  }

</style>