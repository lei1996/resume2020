<script>
import { Radar } from "vue-chartjs";

export default {
  extends: Radar,
  props: {
    radarData: Object,
    options: Object,
  },
  mounted() {
    this.renderChart(
      this.radarData,
      this.options
    );
  }
};
</script>