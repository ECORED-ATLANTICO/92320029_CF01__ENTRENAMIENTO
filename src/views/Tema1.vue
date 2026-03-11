<template lang="pug">
.curso-main-container.pb-3
  BannerInterno
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5.mb-5
    .titulo-principal.color-acento-contenido
      .titulo-principal__numero
        span 1
      h1 Titulo de primer nivel

    .row.align-items-center.mb-5
      .col-md-12.col-sm-12.contain1
        .tema1-block__image1__tema1(
          :style="{'background-image': `url(${require('@/assets/curso/tema1/fot2.png')})`}"
        )
        .tema1-block__image1__logo1(
          :style="{'background-image': `url(${require('@/assets/curso/tema1/logo1.png')})`}"
        )
        .col-md-9.col-sm-10
          .tema1-block__text1
            p.mb-0
                | Los aditivos alimentarios son sustancias que se adicionan intencionalmente a los alimentos con fines tecnológicos durante su producción, para mejorar su conservación, aspecto o sabor. Su uso es tan antiguo como la civilización, aunque su regulación y diversidad han evolucionado drásticamente con el propósito de mantener o mejorar las características físicas, químicas y sensoriales del alimento, sin comprometer la salud del consumidor (FAO & OMS, 2015).
    Separador


    .row.align-items-center.mb-5
      .col-md-12.col-sm-12.contain2
        h2 1.1  Contexto histórico
        .titulo-segundo.color-primario
        .tema1-block__image2__tema1(
          :style="{'background-image': `url(${require('@/assets/curso/tema1/mujer-agrega-sal.svg')})`}"
        )
        .tema1-block__fondo2__tema1(
          :style="{'background-image': `url(${require('@/assets/curso/tema1/fondo1-tema1.png')})`}"
        )
          .col-md-9.col-sm-10
            .tema1-block__text2
              p.mb-0
                  | Desde el Paleolítico, el ser humano ha utilizado aditivos como la sal, el ahumado y el zumo de limón para conservar alimentos. Con el desarrollo de la agricultura y la ganadería, se integraron el azafrán, la sal de nitro y el vinagre para mejorar la palatabilidad y gestionar excedentes.
          .tema1-block__image1__logo2(
          :style="{'background-image': `url(${require('@/assets/curso/tema1/logo2.png')})`}"
          )
        
    
        


</template>

<script>
export default {
  name: 'Tema1',
  data: () => ({
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

<style lang="sass"></style>
