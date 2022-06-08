<template>
      <div class="mainframe">
        <div class="course-text">
          <h1 class="course-text__tittle">Bienvenidos al curso</h1>
          <h2 class="course-text__subtittle">Emprendedores y emprendimiento <br> de El Salvador y la región</h2>
        </div>
        <div class="btn-start animate__animated" @click="animate()">
          <svg xmlns="http://www.w3.org/2000/svg" width="auto" height="auto" viewBox="0 0 110.669 110.224">
            <path d="M0 0c0-81.886-66.38-148.272-148.266-148.272S-296.525-81.886-296.525 0c0 81.879 66.373 148.266 148.259 148.266C-66.38 148.266 0 81.879 0 0Z" style="fill:none;stroke:#36a33d;stroke-width:4;stroke-linecap:round;stroke-linejoin:round;stroke-miterlimit:10;stroke-dasharray:none;stroke-opacity:1" transform="matrix(.35278 0 0 -.35278 109.964 53.01)"/>
            <path style="fill:none;stroke:#fff;stroke-width:4;stroke-linecap:round;stroke-linejoin:round;stroke-miterlimit:10;stroke-dasharray:none;stroke-opacity:1" d="M0 0a157.988 157.988 0 0 0-15.388-2.76" transform="matrix(.35278 0 0 -.35278 69.578 108.093)"/>
            <path style="fill:none;stroke:#fff;stroke-width:4;stroke-linecap:round;stroke-linejoin:round;stroke-miterlimit:10;stroke-dasharray:none;stroke-opacity:1" d="M0 0c-82.401 1.467-149.332 65.307-156.491 145.615" transform="matrix(.35278 0 0 -.35278 55.913 109.518)"/>
            <text xml:space="preserve" style="font-style:normal;font-weight:400;font-size:10.58333302px;line-height:1.25;font-family:sans-serif;letter-spacing:0;word-spacing:0;fill:#f2f2f2;fill-opacity:1;stroke:none;stroke-width:.26458332" x="121.673" y="115.664" transform="translate(-108.707 -50.632)">
            <tspan x="121.673" y="115.664" style="font-style:normal;font-variant:normal;font-weight:700;font-stretch:normal;font-size:28.22222137px;font-family:'Museo Sans';-inkscape-font-specification:'Museo Sans';stroke-width:.26458332;fill:#f2f2f2">Iniciar</tspan>
            </text>
          </svg>
        </div>
        <div class="logos">
          <img src="/v.png" alt="gluss" srcset="">
          <img src="/vuetify-logo.svg" alt="lo que sea" srcset="">
        </div>
      </div>
</template>

<script>
export default {
  name: 'IndexPage',
  methods:{
    animate(){
      const elementoHtml = document.querySelector(".btn-start");
      if(!elementoHtml.classList.contains("animate__bounce")){
        elementoHtml.classList("animate__bounce");
      }
      setTimeout(()=>{elementoHtml.classList.remove("animate__bounce")},1000)
    }
  }
}




</script>

<style>
  .mainframe{
    
    width: 100%;
    height: 100%;
    color:black;
    display: grid;
    grid-template-columns: 5% 45% 20% 25% 5%;
    grid-template-rows: 50% 10% 10% 30%;
  }
  .course-text{
    grid-column-start: 1;
    grid-column-end: 4;
    grid-row-start: 1;
    grid-row-end: 2;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    background-color: #006a36;
    
  }
  .course-text__tittle{
    font-size: 50px;
    font-family: museoSans;
    color: #69b53f;
    align-self: start;
    margin-left: 60px;
  }
  .course-text__subtittle{
    font-size: 50px;
    font-family: museoSanse;
    color: #fdfefe;
    align-self: start;
    margin-left: 60px;
  }
  .btn-start{
    grid-column-start: 4;
    grid-column-end: 5;
    grid-row-start: 1;
    grid-row-end: 2;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    padding: 70px;
    cursor: pointer;
    background-color: #006a36;
  }
  .logos{
    grid-column-start: 3;
    grid-column-end: 5;
    grid-row-start: 3;
    grid-row-end: 4;
  }
</style>