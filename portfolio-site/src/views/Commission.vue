<template>
  <div class="flex-row just-center">
    <div class="flex-col">
      <h1 class="mt-3">Commission Pricing</h1>
      <p>Half payment after sketch and other half when done.</p>
      <br>
      <p>You can reach me through these: </p>

      <ul class="ml-2">
        <li>
          <a href="#">nora.c.hinkle@gmail.com</a>
        </li>
        <li>
          <a href="#">Morffeaus (Discord)</a>
        </li>
        <li>
          <a href="#">morffeaus (Instagram)</a>
        </li>
      </ul>

      <br>
      <p>Payment Methods:</p>
      <ul class="ml-2">
        <li>Paypal (nora.c.hinkle@gmail.com)</li>
        <li>Zelle</li>
        <li>Cashapp</li>
      </ul>

      <div class="card mt-3 ml-1 mr-1">
          <h2 class="card-title">Shading</h2>
            <div class="flex-row just-between">
            <div class="flex-col just-around">
              <h3>Bust: $20</h3>
              <h3>Half: $35</h3>
              <h3>Full: $50</h3>
            </div>
            <div>
              <img src="@/assets/irena-bust.jpg" alt="shadowed bust" class="img-2">
            </div>
        </div>
      </div>

      <div class="card mt-3 ml-1 mr-1">
          <h2 class="card-title">Flat Color</h2>
            <div class="flex-row just-between">
            <div class="flex-col just-around">
              <h3>Bust: $15</h3>
              <h3>Half: $25</h3>
              <h3>Full: $35</h3>
            </div>
            <div>
              <img src="@/assets/axlotl.jpg" alt="shadowed bust" class="img-2">
            </div>
        </div>
      </div>
      
      <div class="card mt-3 ml-1 mr-1 mb-1">
          <h2 class="card-title">Sketch</h2>
            <div class="flex-row just-between">
            <div class="flex-col just-around">
              <h3>Bust: $10</h3>
              <h3>Half: $15</h3>
              <h3>Full: $20</h3>
            </div>
            <div>
              <img src="@/assets/irena-sketch.jpg" alt="shadowed bust" class="img-2">
            </div>
        </div>
      </div>        

    </div>
  </div>
</template>

<script>
export default {
    name: 'Commission'
}
</script>

<style lang="scss" scoped>
div.card{
  background-color: white;
}
</style>