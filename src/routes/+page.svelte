<script>
  import '@arcgis/core/assets/esri/themes/dark/main.css';
  import { defineCustomElements } from '@arcgis/map-components/dist/loader';
  defineCustomElements();
</script>

<!-- create a heatmap from the BuildingPermits layer -->

<arcgis-identity />
<arcgis-map item-id="2876983423be46de943ea05938d01234">
  <arcgis-search position="top-right" />
  <arcgis-legend position="bottom-right" expandable />
  <arcgis-layer-list position="bottom-left" expandable />
  <arcgis-feature-layer
    url="https://services.arcgis.com/V6ZHFr6zdgNZuVG0/arcgis/rest/services/Building_Permits/FeatureServer/0"
    renderer="heatmap"
    opacity="0.75"
  />
</arcgis-map>

<style>
  arcgis-map {
    height: 100vh;
    width: 100vw;
  }
</style>
