<template>
  <div :class="[$style.devEx, 'featureSection']">
    <vue-grid>
      <vue-grid-row>
        <vue-grid-item fill class="vueGridItem">
          <h2>Development Experience</h2>
        </vue-grid-item>
      </vue-grid-row>
      <vue-grid-row>
        <vue-grid-item class="vueGridItem">
          <vue-panel class="vuePanel">
            <vue-panel-body>
              <i class="fas fa-code" />
              <!--<h3>Quick scaffolding</h3>-->
              <p>Como parte de la filosofía de AICAM, Industrial Software Solutions fue creada en 2017 como elemento diferenciador dentro de la transformación digital en la Industria 4.0.</p>
              <p>La transformación digital requiere de elementos que integren conectividad, automatización y optimización digital de procesos y datos. Esto se traduce en una solución software que lo favorece, conectando distintos dispositivos/servicios,  y llevando a sus clientes a una mejora en su eficiencia y progreso</p>
            </vue-panel-body>
          </vue-panel>
        </vue-grid-item>

        <vue-grid-item class="vueGridItem">
          <vue-panel class="vuePanel">
            <vue-panel-body>
              <i class="fas fa-bullhorn" />
              <!--<h3>Instant feedback</h3>-->
              <p>Altran es el proveedor líder mundial en servicios de I + D para sectores vitales como el aeroespacial, defensa, automotriz, semiconductores y electrónica, software e Internet, comunicaciones y ciencias de la vida. En una era en la que el tiempo de comercialización se ha convertido en una obsesión y la disrupción digital es omnipresente, aprovechamos la innovación para ayudar a las compañías a desarrollar y fabricar productos y servicios sin parangón.</p>
            </vue-panel-body>
          </vue-panel>
        </vue-grid-item>
      </vue-grid-row>
    </vue-grid>
  </div>
</template>

<script lang="ts">
  import VueGrid      from '../../shared/components/VueGrid/VueGrid';
  import VueGridItem  from '../../shared/components/VueGridItem/VueGridItem';
  import VueGridRow   from '../../shared/components/VueGridRow/VueGridRow';
  import VuePanel     from '../../shared/components/VuePanel/VuePanel';
  import VuePanelBody from '../../shared/components/VuePanel/VuePanelBody/VuePanelBody';

  export default {
    components: {
      VueGrid,
      VueGridItem,
      VuePanel,
      VuePanelBody,
      VueGridRow,
    },
  };
</script>

<style lang="scss" module>
  @import "../../shared/styles";

  .devEx {
    display:    block;
    text-align: center;

    i {
      display:    inline-block;
      font-size:  $font-size-h1;
      margin-top: $space-unit;
    }

  }
</style>
