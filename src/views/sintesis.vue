<template lang="pug">
.curso-main-container.pb-3
  BannerInterno(icono="fas fa-sitemap" titulo="Síntesis")
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5

    p(data-aos="fade-down").mb-5 El siguiente mapa conceptual integra los criterios y especificidades de los conocimientos expuestos en el presente componente formativo.

    .row.justify-content-center
      .col-12.mb-5
        figure
          img(src="@/assets/curso/temas/sintesis.svg", alt="El manejo de datos consta de: Manejo y protección de datos: se realiza bajo la Ley 1581 del 2012. Maneja un sistema de clasificación de datos donde se tienen las generalidades, implementación, monitoreo y revisión. Estos datos se clasifican en ultrasecreto, secretos, confidenciales, cerrados y abiertos. Instrumentos de recolección de datos: aquí se encuentran las fases de creación de instrumento Hernández Sampieri, en donde se tiene en cuenta, la construcción y uso (instrumentos, formatos), tipos de preguntas (preguntas de tipo cerrado, de tipo abierta o mixta) y aplicación de instrumentos (temporalidad, delimitación de espacio, pregunta mixta, ponderación de alternativas y pertenencias, que genere lenguaje comprensible, inclusión de identificación, formalidad del instrumento, validar la aplicación objetiva). Datos: que tienen en cuenta las variables de información, los principios de clasificación de los datos e información (apertura, transparencia y valores sociales, datos con contenido y neutrales, enfoque de gestión de riesgo, proporcionalidad, funciones y responsabilidades, enfoque del ciclo de vida) y los tipos de datos y agrupación (datos cuantitativos continuos y discretos, datos cualitativos dicotómicos y politómicos). Fuentes y técnicas de recolección de información: con sus tipos de fuentes de información (fuentes primarias, secundarias, terciarias) y técnicas de recolección de información (entrevista, encuesta, análisis documental, observación no experimental y observación experimental).")
      .col-auto
        a.anexo.mb-4(:href="obtenerLink('/downloads/Sintesis.pdf')" target="_blank")
          .anexo__icono
            img(src="@/assets/template/icono-pdf.svg")
          .anexo__texto
            p Anexo. Síntesis

</template>

<script>
export default {
  name: 'Sintesis',
  data: () => ({
    // variables de vue
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
