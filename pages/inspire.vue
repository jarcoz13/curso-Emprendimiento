<template>
  
  <div class="containerOne">
      <div class="hamburger">
        <div class="hamburger-inner"></div>
      </div>  
      <div class="titulo">
        <h3 class="textoCurso">Curso: Emprendedor y emprendimiento en el Salvador y la Región</h3>
      </div>
      
      <div class="pagina">
         Pagina 1 de 20
      </div>
    
      <div class="logos2">
        <img class="bancoPopular" src="/banco_popular.png" alt="banco popular" srcset="">
        <img src="/iniciativa-dinamica.png" alt="inciatiba dinamica" srcset="">
      </div>
      <div clas="piePAgina">
        <img class=""
      </div>

  </div>
</template>

<script>
export default {
  name: 'InspirePage',
  layout: 'startLayout',
  data(){
      return{
      hola:"hola"
    }
  }
}
</script>
<style >
.containerOne{
  background-color: white;
  grid-template-columns: 3% 27% 10% 10% 49% 1% ;
  grid-template-rows: 20% 10% 60% 10%;
  width: 100%;
  height: 100%;
  display: grid;
  color: black;
}


.hamburger {
    min-height: 20px;
    max-width: 30px;
    grid-column-start: 1;
    grid-column-end: 2;
    grid-row-start: 1;
    grid-row-end: 3;
    background-color: #c3c5cb;
}
.hamburger-inner, .hamburger-inner:after, .hamburger-inner:before {
    background-color: #096f50;
    position: absolute;
    width: 20px;
    height: 3px;
    border-radius: 5px;
    content: '';
    transition-timing-function: ease;
    transition-duration: .2s;
    transition-property: transform,opacity;
}
.hamburger-inner:before {
    top: 5px;
}
.hamburger-inner:after {
    top: 10px;
}

.titulo{
  background-color: #006a36;
  grid-column-start: 5;
  grid-column-end: 6;
  grid-row-start:1 ;
  grid-row-end: 2;
  color: #e6f0ea;
  font-size: smaller;
  align-items: right ;

}
.textoCuros{
  align-self:;
  margin-right: 100px;
}
.pagina{
  background-color: #ffffff;
  color: #137140;
  box-sizing: content-box;  
  
  border: 2px solid #c6e238;
  grid-column-start: 5;
  grid-column-end: 6;
  grid-row-start: 2;
  grid-row-end: 3;
  width: 120px;
  height: 30px;
  
}
.logos2{
    grid-column-start: 2;
    grid-column-end: 3;
    grid-row-start:1 ;
    grid-row-end: 2;
    width: 30px;
    height: 90px;
    display: flex;
    flex-direction: row;  
  }
</style>