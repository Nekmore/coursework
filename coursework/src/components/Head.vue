    <template>
      <section>
        <menu>
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
        </menu>
      </section>
    </template>

    <script>

    </script>

    <style>
      menu {
        padding: 0;
        display: grid;
        grid-template-columns: 0.1fr 0.2fr 3fr 0.2fr 0.2fr;
        grid-template-rows: 50px;
        grid-gap: 0.5vw;
        align-items: center;
        justify-items: center;



      }

      .logo {
        width: 35px;
        height: 35px;
        border-radius: 40px;
        background: red;
      }

      .main {
        width: 100%;
      }

      .main > input {
        width: 100%;
        height: 38px;
        border-radius: 40px;
        border: none;
        background: black;
        color: white;
      }

      .search {
        width: 100%;
      }

      .search > input {
        width: 100%;
        height: 38px;
        border-radius: 40px;
        padding-left: 15px;
        border: none;
        background: #BBBBBB;
        color: white;

      }

      .login {
        width: 100%;
        justify-self: right;
        display: grid;
        justify-items: right;
      }

      .login > input {
        width: 80%;
        height: 38px;
        border: none;
        border-radius: 40px;
        background: none;
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
        height: 38px;
        justify-self: right;
        border: none;
        border-radius: 40px;
        background: none;
      }

      .registration > input:hover {
        background: red;
        color: white;
      }
    </style>