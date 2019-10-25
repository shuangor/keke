<template>
  <div class="hello">
    <div v-bind:class="{change: one}">
      <img src="../assets/111.png" />
      <div style="width: 100%;height: 50px;"></div>
      <div class="top">
        第一次见面那次饭桌上，你无意间的回目一笑，便留在了我脑海里，我知道我陷进去了，前段时间听说你相亲谈崩了，深知要抓住这次机会
      </div>
      <div class="center">
        吕可，我喜欢你
      </div>
      <div class="footer" style="color: white;width: 250px;height: 60px;margin: 60px auto;background-color: black;opacity: 0.6;line-height: 60px;font-size: 20px;border-radius: 6px;">做我女朋友吧！</div>
    </div>
    <!-- <div class="showimg" v-bind:class="{change: two}" style="width: 100%; height: 100%; background-color: white;">
      <img src="../assets/111.png" />
      <div style="position: absolute;width: 500px; height: 700px;background-color: red;">
        
      </div>
    </div> -->
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  data() {
    return {
      one: false,
      two: true
    }
  },
  methods: {
    changepage() {
      this.one = true;
      this.two = false;
    }
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.change {
  display: none;
}

.hello {
  position: relative;
  width: 100%;
  height: 100vh;
  background-color: rgba(0, 0, 0, 0.3);
}
img {
  position: absolute;
  top: 0px;
  left: 0px;
  width: 100%;
  height: 100vh;
  z-index: -110;
}

.top {
  width: 75%;
  height: 85px;
  padding-left: 10px;
  padding-right: 10px;
  padding-top: 15px;
  padding-bottom: 15px;
  background-color: #8B7765;
  margin: 0px auto;
  text-align: left;
  color: rgb(240, 240, 240);
  letter-spacing: 1.5px;
  text-indent: 2em;
  box-shadow: 2px 2px 5px #BDBDBD;
  border-radius: 12px;
}

.center {
  width: 80%;
  height: 90px;
  line-height: 90px;
  font-size: 22px;
  margin: 0px auto;
  margin-top: 100px;
  color: #EEA2AD;
  letter-spacing: 2px;
  background-color: rgba(0, 0, 0, 0.5);
}

.showimg > img {
  position: absolute;
  top: 0px;
  left: 0px;
  width: 100%;
  height: 100vh;
  z-index: 10;
}


</style>
