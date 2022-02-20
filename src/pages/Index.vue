<template>
  <q-page class="flex flex-center"> <chartMe />y </q-page>
</template>

<script>
import { defineComponent, defineAsyncComponent } from "vue";
const chartMe = defineAsyncComponent(() =>
  import("components/charts/mychart.vue")
);
export default defineComponent({
  name: "PageIndex",
  components: {
    chartMe,
  },
});
</script>
