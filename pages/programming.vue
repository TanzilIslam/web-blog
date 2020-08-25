<template>
  <div class="pt-3">
    <div class="d-flex pb-4">
      <b-card
        no-body
        img-height="50"
        img-width="50"
        class="rounded"
        img-src="~/assets/cover-one.png"
      ></b-card>
      <h4><strong>Programming Posts</strong></h4>
    </div>
    <b-row>
      <b-col v-for="i in 6" :key="i" cols="12" sm="6" md="4" lg="4" xl="4">
        <SmallCard />
      </b-col>
    </b-row>
  </div>
</template>

<script>
import SmallCard from '@/components/SmallCard.vue'
export default {
  components: {
    SmallCard,
  },
}
</script>

<style></style>
