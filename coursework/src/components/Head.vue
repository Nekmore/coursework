<template>
  <section>
    <nav>
      <div class="logo">
      </div>
      <div class="main">
        <input type="button" value="Главная">
      </div>
      <div class="search">
        <input type="text" placeholder="Поиск">
      </div>
      <div class="login">
        <input type="button" value="Вход">
      </div>
      <div class="registration">
        <input type="button" value="Регистрация">
      </div>
    </nav>
  </section>
</template>

<script>

</script>

<style>
  nav {
    padding: 0;
    display: grid;
    grid-template-columns: 0.1fr 0.2fr 3fr 0.2fr 0.2fr;
    grid-template-rows: 3vw;
    grid-gap: 0.5vw;
    align-items: center;
    justify-items: center;
  }

  .logo {
    width: 2vw;
    height: 2vw;
    border-radius: 40px;
    background: red;
  }

  .main {
    width: 100%;
  }

  .main > input {
    width: 100%;
    height: 2vw;
    border-radius: 40px;
    border: none;
    background: black;
    color: white;
    font-size: 0.7vw;
  }

  .search {
    width: 100%;
  }

  .search > input {
    width: 100%;
    height: 2vw;
    border-radius: 40px;
    padding-left: 15px;
    border: none;
    background: #BBBBBB;
    color: white;
    font-size: 0.7vw;

  }

  .search > input:focus {
    outline: none;
  }

  .login {
    width: 100%;
    justify-self: right;
    display: grid;
    justify-items: right;
  }

  .login > input {
    width: 80%;
    height: 2vw;
    border-radius: 40px;

    border: none;
    background: none;
    font-size: 0.7vw;
  }

  .login > input:hover {
    background: red;
    color: white;
  }


  .registration {
    width: 100%;
    justify-self: right;
  }

  .registration > input {
    width: 100%;
    height: 2vw;
    justify-self: right;
    border: none;
    border-radius: 40px;
    background: none;
    font-size: 0.7vw;
  }

  .registration > input:hover {
    background: red;
    color: white;
  }
</style>