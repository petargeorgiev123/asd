<template>
  <div :class="[$style.quickStart, 'featureSection']">
    <vue-grid>
      <vue-grid-row>
        <vue-grid-item fill class="vueGridItem">
          <h2>Digital Transformation</h2>
        </vue-grid-item>

        <vue-grid-item class="vueGridItem">
          <vue-panel class="vuePanel">
            <vue-panel-body class="vuePanelBody">
              <ol>
                <li>Industrial Communication networks</li>
                <li>IoT</li>
                <li>Big Data</li>
                <li>Factory Analitics</code></li>
                <li>Artifical Intelligence</li>
                <li>Newural Networks</li>
                <li>Industrial Information Systems</li>
                <li>Cybersecurity</li>
              </ol>
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
  import VuePanel     from '../../shared/components/VuePanel/VuePanel';
  import VuePanelBody from '../../shared/components/VuePanel/VuePanelBody/VuePanelBody';
  import VueGridRow   from '../../shared/components/VueGridRow/VueGridRow';

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

  .quickStart {
    display:    block;
    text-align: center;
    @include background-gradient($brand-dark-primary, $brand-primary, -31deg);

    :global {
      .vuePanelBody {
        text-align: left;
        overflow:   hidden;

        ol {
          margin-top: $space-unit * 5;
          padding:    0 0 0 $space-unit * 2;

          li {
            margin-bottom: $space-unit * 2;
          }
        }
      }
    }

    @include media(tabletPortrait) {
      :global {
        .vuePanel {
          width:       50%;
          margin-left: 25%;
        }
      }
    }

    @include media(tabletLandscape) {
      :global {
        .vuePanel {
          width:       33.3333333%;
          margin-left: 33.3333333%;
        }
      }
    }
  }
</style>
