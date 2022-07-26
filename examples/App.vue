<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
<Demo></Demo>
    <Card imgSrc="AI.png"
    summary="AI Learn">
    </Card>
    <br/>
    <Card imgSrc="agile.png"
          summary="agile Learn">
      <template v-slot:footer>
        <div class="m-card-footer">
          <div class="level">
            dfdf
          </div>
          <div class="price">$299.00</div>
        </div>
      </template>
    </Card>
    <br/>
    <Card imgSrc="always-on.png"
          :width="370"
          :imgHeight="90"
          >
      summary="always-on Learn"
      <template v-slot:footer>
        <div class="m-card-footer-spring">
          <div class="level">
            jkdlf
          </div>
          <div class="level">
dfdf
          </div>
        </div>
      </template>
    </Card>

  </div>
</template>

<script>

export default {
  name: 'App',
  components: {
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.m-card-footer {
  padding: 0 8px;
  font-size: 12px;
  text-align: left;
}

.level {
  color: #9199a1;
  margin-bottom: 8px;
}

.price{
  color: #f01414;
}

.m-card-footer-spring {
  display: flex;
  justify-content: space-between;
  padding: 0 8px;
  font-size: 12px;
}
</style>
