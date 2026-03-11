<template lang="pug">
.curso-main-container.introduccion
  BannerInterno
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5.mb-5
    .titulo-principal.color-acento-contenido
      .titulo-principal__numero
        span i
      h1 Introducción

    .row.align-items-center.mb-5
      .col-md-3.col-sm-12
        .intro-block__image(
          :style="{'background-image': `url(${require('@/assets/curso/introduccion/fot1.svg')})`}"
        )
      .col-md-9.col-sm-12
        .intro-block__text
          p.mb-0
            | Los alimentos procesados hacen parte fundamental de la dieta actual y su calidad depende, en gran medida, de los procesos y sustancias empleadas durante su elaboración. Entre estos elementos se encuentran los aditivos alimentarios, compuestos que cumplen funciones tecnológicas específicas y que inciden directamente en la estabilidad, apariencia, sabor e inocuidad de los productos.
    
    
    .row.align-items-center.mb-5
      .col-md-12.col-sm-12.azulC
        .intro-block__image-Masc(
          :style="{'background-image': `url(${require('@/assets/curso/introduccion/estrellaA.png')})`}"
        )
        .intro-block__image-Micro(
          :style="{'background-image': `url(${require('@/assets/curso/introduccion/micro.svg')})`}"
        )

        .col-md-8.col-sm-12
          .intro-block__text2
            p.mb-0
              | Comprender el origen, la clasificación, la función y la regulación de los aditivos permite interpretar de manera adecuada los análisis físicoquímicos aplicados a los alimentos y tomar decisiones informadas dentro de los procesos de control de calidad. Este componente desarrolla los conceptos esenciales y su aplicación práctica, promoviendo el uso responsable y normado de los aditivos en coherencia con las exigencias del sector alimentario.
    
    
    .row.align-items-center.mb-5
      .col-md-12.col-sm-12.azulOs
        .podcast-content
          .podcast-image(
            :style="{'background-image': `url(${require('@/assets/curso/introduccion/podc.svg')})`}"
          )
          .podcast-player
            .podcast-title Pódcast
            .tarjeta-audio-container
              TarjetaAudio.color-primario(
                texto="Etiquetas bajo la lupa"
                :audio="require('@/assets/componentes/audios/audio-ej.mp3')"
              )

</template>

<script>
export default {
  name: 'Introduccion',
  data: () => ({
    mostrarIndicadorAudio: true,
    mostrarIndicadorTarjetaAudio: true,
  }),
  mounted() {
    this.$nextTick(() => {
      this.$aosRefresh()
    })
  },
  updated() {
    this.$aosRefresh()
  },
}
</script>

<style lang="sass">
.bloque-texto-g__img
  width: 300px !important
  height: 104px !important
  border-radius: 15px
  background-size: cover !important
  background-position: center !important
</style>
