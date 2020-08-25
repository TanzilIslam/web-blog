<template>
  <div class="pt-3">
    <Carousel class="mb-4" />
    <b-row>
      <b-col
        v-for="i in 5"
        :key="i"
        cols="12"
        sm="12"
        md="8"
        lg="8"
        offset-lg="2"
        offset-md="2"
        offset-xl="2"
        xl="8"
      >
        <HomeCard />
      </b-col>
    </b-row>
  </div>
</template>

<script>
import HomeCard from '@/components/HomeCard.vue'
export default {
  components: {
    HomeCard,
  },
}
</script>

<style></style>
