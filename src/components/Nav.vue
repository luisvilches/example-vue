<script>
  export default {
    name: 'Navbar'
  }
</script>

<template>
  <nav class="principal">
    <div class="container pdheader">
      <div class="row">
        <div class="col-md-4 col-xs-12 logo">
          <router-link to="/"><h3>Ibatido</h3></router-link>
          <router-link to="/"><p>Distribuidor independiente Herbalife</p></router-link>
        </div>
        <div class="col-md-4 col-xs-12">
          <input type="text" id="search" placeholder="Buscar..." class="form-control">
        </div>
        <div class="col-md-4">
          <ul class="login">
              <li class="shopicon"><router-link to="/cart"><i class="fa fa-shopping-bag" aria-hidden="true"></i><span class="badge badge-secondary">0</span></router-link></li>
            <li><router-link to="/login">Iniciar sesion</router-link></li>
            <li>|</li>
            <li><router-link to="/register">Registrarse</router-link></li>
          </ul>
        </div>
      </div>
    </div>
  </nav>
</template>

<style scoped>
  .pdheader ul.login li {
      display: inline-block;
      margin-left: 5px;
      position: relative;
      top: 18px;
  }

  .pdheader ul.login li a{
      color: #fff;
      text-decoration: none;
      font-size: 13px;
  }

  .pdheader ul li a:hover{
      color: #24babc;
  }

  .pdheader ul {
      text-align: right;
      margin-right: 10px;
      padding-bottom: 8px; 
  }

  nav.principal{
      position: fixed;
      top:0;
      width: 100%;
      z-index: 999999999;
      background: #32373d;
      color: white;
      padding-top: 0px;
      border-bottom: 1px solid #2d2d2d;
  }

  .list-header li{
      display: inline-block;
      margin-left: 5px;
      list-style: none;
      font-size: 16px;
  }

  .shopicon a i{
      font-size: 30px;
      margin-left: 40px;
  }

  .shopicon a{
      color: #fff;
  }

  .shopicon a:hover{
      color: #2d2d2d;
  }

  .shopicon span{
      border-radius: 100px;
      margin-left: -8px;
      background: #444;
  }

  #search{
      border-radius: 50px;
      border: 1px solid transparent;
      position: relative;
      top: 18px;
  }
  .pdheader .logo h3{
      margin-top: -5px;
  }

  .logo a{
      text-decoration: none;
      position: relative;
      top: 10px;
  }
  .logo h3{
      font-style: italic;
      font-size: 50px;
      color: #fff;
      font-family: "AvenirNextLTPro-Regular";
  }
  .logo p{
      margin-top: -20px;
      font-size: 10px;
      color: #fff;
      font-family: "AvenirNextLTPro-Regular";
  }

  .pdheader{
      padding: 10px 0px;
      
  }


  

  @media (max-width: 768px){
      .login ul{
          text-align: center;
          margin-right: 0px;
      }

      .list-header li{
          margin-top: 10px;
          text-align: center;
          margin-left: 0px;
      }

      .shopicon i{
          text-align: center;
          margin-left: 0px;
      }
      
      .shopicon span{
          text-align: center;  
      }

      .principal{
        text-align: center;
        padding: 20px;
      }

      ul.login{
        margin-top: 15px;
        text-align: center;
      }
  }

  nav.secondary{
      height: 40px;
      background: #fff;
  }

  nav.secondary ul li{
      list-style: none;
      display: inline-block;
      margin-left: 10px;
      margin-right: 10px;
  }

  nav.secondary ul{
      text-align: center;
      padding: 5px;
  }
</style>
