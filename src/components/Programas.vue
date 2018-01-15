<script>
    export default {
        name:"destacados",
        data(){
            return{
                products:[]
            }
        },
        created: function(){
            this.products = [
                    {
                        name:"PLAN PRUEBA 15 DÍAS",
                        price:"1 batido, 1 proteína, 1 té Thermojetics 50g",
                        img:"http://www.tubienestar.cl/wp-content/uploads/2015/04/Herbalife-2B1A.jpg"
                    },
                    {
                        name:"ECONOMICO",
                        price:"2 batidos",
                        img:"http://productos.herbalife.cl/Content/es-CL/img/Productos/BATIDO_VAINILLA_CL.jpg"
                    },
                    {
                        name:"MÁXIMOS RESULTADOS",
                        price:"2 batidos, 2 proteínas",
                        img:"https://nutricionycontroldepeso.cl/wp-content/uploads/2016/04/Proteina_2017.jpg"
                    },
                    {
                        name:"QUEMA GRASAS",
                        price:"2 batidos, 2 proteínas 1 Té Thermojetics.",
                        img:"http://www.tubienestar.cl/wp-content/uploads/2015/04/Herbalife-2B1A.jpg"
                    },
                    {
                        name:"QUEMA GRASAS Y ATRAPA GRASAS",
                        price:"2 batidos, 2 proteínas 1 Té Thermojetics, 1 Lipo Bond.",
                        img:"http://productos.herbalife.cl/Content/es-CL/img/Productos/BATIDO_VAINILLA_CL.jpg"
                    }
                ]
        },
        methods:{},
        components:{}
    }
</script>
<template>
    <div class='container'>
        <div class="row">
            <div class="col-md-12">
                <h3 class="text-center">BAJA DE PESO CON ESTOS PROGRAMAS</h3>
                <h5 class="text-center">CONTROL DE PESO Y NUTRICIÓN</h5>
                <br>
            </div>
        </div>
        <div class="row">
            <div class="col" v-for="item in products">
                <div class='card'>
                    <div class='card-content'>
                        <div class='top-bar'>
                            <span>
                                {{item.name}}
                            </span>
                            <span class='float-right lnr lnr-heart'></span>
                        </div>
                        <div class='img'>
                            <img v-bind:src="item.img">
                        </div>
                    </div>
                    <div class='card-description'>
                        <div class='title'>
                            {{item.price}}
                        </div>
                    </div>
                    <div class='cart text-center'>
                        <a class="green">ver mas</a>
                        <br>
                        <br>
                    </div>
                </div>
            </div>
        </div>  
    </div>
</template> 

<style scoped>
        .container{
    margin-top: 60px;
    margin-bottom: 60px;
}

.card {
    width:100%;
    max-height: 400px;
  position: relative;
  padding: 0px;
  background: white;
  display: grid;
  grid-template-rows: 8fr 1fr 1fr;
  -webkit-box-shadow: 0px 15px 20px 0px rgba(0, 0, 0, 0.057);
          box-shadow: 0px 15px 20px 0px rgba(0, 0, 0, 0.057);
  -webkit-transition: 0.2s ease-in;
  transition: 0.2s ease-in;
}
.card .card-content {
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-pack: center;
      -ms-flex-pack: center;
          justify-content: center;
  -webkit-box-align: center;
      -ms-flex-align: center;
          align-items: center;
  width: 100%;
}
.card .card-content .top-bar {
  width: calc(100% - 40px);
  position: absolute;
  top: 0;
  left: 0;
  padding: 20px;
}
.card .card-content .top-bar span {
    font-size:12px;
}
.card .card-content .top-bar .float-right {
  float: right;
}
.card .card-content .img {
  width: 100%;
  -webkit-box-pack: bottom;
      -ms-flex-pack: bottom;
          justify-content: bottom;
  -ms-flex-line-pack: bottom;
      align-content: bottom;
  text-align: center;
}
.card .card-content .img img {
  max-width: 100%;
  max-height: 220px;
  margin-top:40px;
}
.card .card-description {
  padding: 10px;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-pack: justify;
      -ms-flex-pack: justify;
          justify-content: space-between;
  -webkit-box-align: center;
      -ms-flex-align: center;
          align-items: center;
  font-weight: 400;
  font-size: 14px;
  letter-spacing: 0.1em;
  width: calc(100%-20px);
}
.card .card-description .title {
  text-transform: uppercase;
  text-align: center;
  font-size: 10px;
}
.card .card-description .cart {
  float: right;
  cursor: pointer;
}
.card .card-footer {
  text-transform: uppercase;
  padding: 0.3em;
  border-top: 0.5px solid #ececec;
  letter-spacing: 0.1em;
  font-size: 11px;
  color: white;
  justify-items: left;
  -webkit-box-align: center;
      -ms-flex-align: center;
          align-items: center;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
}
.card .card-footer .span {
  margin: 5px;
  width: auto;
  background: #dedede;
  padding: 4px 7px;
  border-radius: 2px;
  font-weight: 100;
  cursor: pointer;
}
.card .card-footer .span:hover {
  background: #aaaaaa;
}
.card:hover {
  -webkit-transition: 0.2s ease-in;
  transition: 0.2s ease-in;
  -webkit-transform: translateY(-10px);
          transform: translateY(-10px);
  -webkit-box-shadow: 0px 45px 60px 0px rgba(0, 0, 0, 0.087);
          box-shadow: 0px 45px 60px 0px rgba(0, 0, 0, 0.087);
}


.allproducts{
    margin: 20px;
    padding: 15px;
    background: #24babc;
    border: 1px solid transparent;
}

.green{
    color:#24babc !important;
}
</style>