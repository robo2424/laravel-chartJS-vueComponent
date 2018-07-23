<script>
import { Line } from 'vue-chartjs'
 
export default {
  extends: Line,
  mounted () {
      console.log('Example Chart mounted successfully')
    // Overwriting base render method with actual data.
    this.renderChart({
      labels: ['January', 'February', 'March', 'April', 'May', 'June', 'July', 'August', 'September', 'October', 'November', 'December'],
      datasets: [
        {
          label: 'Sales By Month',
          backgroundColor: '#d9d9d9',
          data: [40, 20, 12, 39, 10, 40, 39, 80, 40, 20, 12, 11]
        }
      ]
    })
  }
}
</script>