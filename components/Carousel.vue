<template>
  <div class="pt-1">
    <b-carousel
      id="carousel-1"
      v-model="slide"
      :interval="4000"
      controls
      indicators
      background="white"
      img-width="1024"
      img-height="300"
      @sliding-start="onSlideStart"
      @sliding-end="onSlideEnd"
    >
      <b-carousel-slide class="custom-slide">
        <template v-slot:img>
          <img
            class="d-block img-fluid w-100"
            width="1024"
            height="300"
            src="~/assets/cover-one.png"
            alt="image slot"
          />
        </template>
        <h4>Web Technology</h4>
      </b-carousel-slide>
      <b-carousel-slide class="custom-slide">
        <template v-slot:img>
          <img
            class="d-block img-fluid w-100"
            width="1024"
            height="300"
            src="~/assets/cover2.png"
            alt="image slot"
          />
        </template>
        <h4>Future Library</h4>
      </b-carousel-slide>
      <b-carousel-slide class="custom-slide">
        <template v-slot:img>
          <img
            class="d-block img-fluid w-100"
            width="1024"
            height="300"
            src="~/assets/cover-three.png"
            alt="image slot"
          />
        </template>
        <h4>Easy to access</h4>
      </b-carousel-slide>
    </b-carousel>
  </div>
</template>

<script>
export default {
  data() {
    return {
      slide: 0,
      sliding: null,
    }
  },
  methods: {
    onSlideStart(slide) {
      this.sliding = true
    },
    onSlideEnd(slide) {
      this.sliding = false
    },
  },
}
</script>
<style scoped>
.custom-slide img {
  height: 350px !important;
  border-radius: 5px !important;
}
</style>
