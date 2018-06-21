<template>
  <div class="container py-2">
    <div class="row my-2">
      <div class="col">
        <h3>Overview</h3>
      </div>
    </div>

    <div class="row mb-2">
      <div class="col">
        <div class="card">
          <div class="card-body text-center">
            <div class="d-flex justify-content-center align-items-center">
              <i class="fas fa-hand-holding-usd"></i>
              <h6 class="ml-1 mb-0">TOTAL REVENUE</h6>
            </div>
            <h2>12,345</h2>
          </div>
        </div>
      </div>
      <div class="col">
        <div class="card">
          <div class="card-body text-center">
            <div class="d-flex justify-content-center align-items-center">
              <i class="fas fa-th-large"></i>
              <h6 class="ml-1 mb-0">TOTAL COST</h6>
            </div>
            <h2>12,345</h2>
          </div>
        </div>
      </div>
      <div class="col">
        <div class="card">
          <div class="card-body text-center">
            <div class="d-flex justify-content-center align-items-center">
              <i class="fas fa-money-bill-alt"></i>
              <h6 class="ml-1 mb-0">NET INCOME</h6>
            </div>
            <h2>12,345</h2>
          </div>
        </div>
      </div>
    </div>

    <div class="row mb-2">
      <div class="col">
        <div class="card">
          <div class="card-body">
            <h5>Activity</h5>
            <LineChart :data="lineData" :options="lineOptions"></LineChart>
          </div>
        </div>
      </div>
    </div>

    <div class="row">
      <div class="col">
        <div class="card">
          <div class="card-body">
            <h5>Transaction Website</h5>
            <ul class="list-group list-group-flush">
              <li class="list-group-item py-4 border-top-0 d-flex justify-content-between">
                <div class="d-flex align-items-center">
                  <i class="fab fa-facebook-square fa-3x"></i>
                  <h6 class="ml-4 mb-0">Facebook.com</h6>
                </div>
                <div class="d-flex align-items-center">
                  <h4 class="mr-4 mb-0">45,836</h4>
                  <i class="fas fa-arrow-up"></i>
                  <p class="ml-1 mb-0">20%</p>
                </div>
              </li>
              <li class="list-group-item py-4 d-flex justify-content-between">
                <div class="d-flex align-items-center">
                  <i class="fab fa-google fa-3x"></i>
                  <h6 class="ml-4 mb-0">Google.com</h6>
                </div>
                <div class="d-flex align-items-center">
                  <h4 class="mr-4 mb-0">45,836</h4>
                  <i class="fas fa-arrow-up"></i>
                  <p class="ml-1 mb-0">20%</p>
                </div>
              </li>
              <li class="list-group-item py-4 d-flex justify-content-between">
                <div class="d-flex align-items-center">
                  <i class="fab fa-apple fa-3x"></i>
                  <h6 class="ml-4 mb-0">Apple.com</h6>
                </div>
                <div class="d-flex align-items-center">
                  <h4 class="mr-4 mb-0">45,836</h4>
                  <i class="fas fa-arrow-up"></i>
                  <p class="ml-1 mb-0">20%</p>
                </div>
              </li>
              <li class="list-group-item py-4 d-flex justify-content-between">
                <div class="d-flex align-items-center">
                  <i class="fab fa-wordpress-simple fa-3x"></i>
                  <h6 class="ml-4 mb-0">Wordpress.com</h6>
                </div>
                <div class="d-flex align-items-center">
                  <h4 class="mr-4 mb-0">45,836</h4>
                  <i class="fas fa-arrow-up"></i>
                  <p class="ml-1 mb-0">20%</p>
                </div>
              </li>
            </ul>
          </div>
        </div>
      </div>
      <div class="col">
        <div class="card">
          <div class="card-body">
            <h5>Latest Orders</h5>
            <ul class="list-group list-group-flush">
              <li class="list-group-item border-top-0 d-flex align-items-end">
                <img
                  src="https://images.unsplash.com/photo-1503341455253-b2e723bb3dbb?ixlib=rb-0.3.5&ixid=eyJhcHBfaWQiOjEyMDd9&s=68844cdf917d32eb1b90c2537e9c1c5f&auto=format&fit=crop&w=1350&q=80"
                  class="last-order-img img-thumbnail">
                <div class="ml-3">
                  <h5>Vintage T-shirt</h5>
                  <p class="mb-0">Vintage T-shirt</p>
                  <p class="mb-0">Belle Wills</p>
                </div>
                <div class="ml-auto">
                  <h6 class="text-right">Total</h6>
                  <h4 class="mb-0">3,200</h4>
                </div>
              </li>
              <li class="list-group-item d-flex align-items-end">
                <img
                  src="https://images.unsplash.com/photo-1520975867597-0af37a22e31e?ixlib=rb-0.3.5&ixid=eyJhcHBfaWQiOjEyMDd9&s=8cbd3e929d64dbadf80ab85bb9b52762&auto=format&fit=crop&w=634&q=80"
                  class="last-order-img img-thumbnail">
                <div class="ml-3">
                  <h5>Cowboy Jacket</h5>
                  <p class="mb-0">Cowboy Jacket</p>
                  <p class="mb-0">Adrian Cummings</p>
                </div>
                <div class="ml-auto">
                  <h6 class="text-right">Total</h6>
                  <h4 class="mb-0">2,800</h4>
                </div>
              </li>
              <li class="list-group-item d-flex align-items-end">
                <img
                  src="https://images.unsplash.com/photo-1515603848232-f52a8e50511a?ixlib=rb-0.3.5&ixid=eyJhcHBfaWQiOjEyMDd9&s=830067c15934777bed04a47c8259a162&auto=format&fit=crop&w=614&q=80"
                  class="last-order-img img-thumbnail">
                <div class="ml-3">
                  <h5>Coach Coat</h5>
                  <p class="mb-0">Coach Coat</p>
                  <p class="mb-0">Lura Holland</p>
                </div>
                <div class="ml-auto">
                  <h6 class="text-right">Total</h6>
                  <h4 class="mb-0">1,600</h4>
                </div>
              </li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import LineChart from '~/components/line-chart'

export default {
  layout: 'admin',
  components: {
    LineChart
  },
  data () {
    return {
      lineData: {
        labels: ['January', 'February', 'March', 'April', 'May', 'June', 'July', 'Aug'],
        datasets: [
          {
            label: 'Total Revenue',
            backgroundColor: '#7ED321',
            borderColor: '#7ED321',
            data: [7222, 6914, 5769, 7256, 5769, 6125, 7256, 7212]
          },
          {
            label: 'Total Cost',
            backgroundColor: '#D0021B',
            borderColor: '#D0021B',
            data: [500, 505, 2701, 2904, 2401, 575, 778, 2003]
          },
          {
            label: 'Net Income',
            backgroundColor: '#4A90E2',
            borderColor: '#4A90E2',
            data: [6124, 5255, 2001, 3994, 3812, 5598, 6223, 4993]
          }
        ]
      },
      lineOptions: {
        maintainAspectRatio: false,
        elements: {
          line: {
            fill: false,
            tension: 0, // disables bezier curves
          }
        }
      }
    }
  },
}
</script>

<style lang="scss">
.last-order-img {
  width: 100px;
  height: 100px;
}
</style>
