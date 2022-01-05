<template>
<div class="">
  <div class="slider">
    <div class="slider-description">
      <h2>Долго, дорого, скрупулезно.</h2>
      <p>Математически выверенный дизайн <br>для вашего сайта или мобильного приложения.</p>
      <button>Узнать больше</button>
      <section class='radio'>
        <input type="radio" name='slider' value="1" v-model="value" @click="change">
        <input type="radio" name='slider' value="2" v-model="value" @click="change">
        <input type="radio" name='slider' value="3" v-model="value" @click="change">
      </section>
    </div>
    <img :src='SliderItem' width="760" height="431" alt="Slide1">
      </div>
  <p>Slider</p>
</div>
</template>

<script>
import './Slider.less';
export default {
  name: 'Slider',
  data() {
    return {
      value: 1,
    }
  },
  methods: {
    // change: function() {
    // },
  },
  computed: {
    SliderItem(){
      return require(`@/assets/img/slide${this.value}.png`)
    }
  },
  props: {}
}
</script>

<style scoped>
.slider {
  margin: 0;
  padding: 0;
  margin: auto;

  width: 100%;
  background: #eeeeee;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
}

.slider-description {
  margin: 0;
  padding: 0;
  margin: 80px;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}

.slider-description h2 {
  margin: 0;
  padding: 0;

  font-size: 36px;
  line-height: 36px;
  font-weight: 500;
  color: #000;
}

.slider-description p {
  margin: 42px 0;

  font-weight: 400;
  font-size: 12px;
  line-height: 22px;
}

.slider-description button {
  margin: 0;
  padding: 0;
  padding: 12px 35px;
  background: #fb565a;
  cursor: pointer;
  color: #fff;
  border: none;
}

.radio {
  margin: 0;
  margin-top: 30px;
  padding: 0;
  display: flex;
  flex-direction: row;
  justify-content: center;
  color: transparent;
}
</style>
