<template>
  <div class="pt-3">
    <Carousel class="mb-4" />
    <b-row>
      <b-col
        v-for="(item, index) in results"
        :key="index"
        cols="12"
        sm="12"
        md="8"
        lg="8"
        offset-lg="2"
        offset-md="2"
        offset-xl="2"
        xl="8"
      >
        <HomeCard :article="item" />
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
  async fetch() {
    const self = this
    await self.$axios
      .$get(process.env.baseUrl)
      .then(function (posts) {
        self.results = posts.results
      })
      .catch(function (e) {
        // eslint-disable-next-line no-console
        console.log(e)
      })
  },
  data() {
    return {
      results: {},
    }
  },
}
</script>

<style></style>
