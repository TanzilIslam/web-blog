<template>
  <div class="pt-3">
    <h4 class="pt-2 ml-5"><strong>#Author List</strong></h4>
    <b-row>
      <b-col cols="3" sm="6" md="3" lg="3" xl="3">
        <b-list-group class="custom-list-gropu">
          <b-list-group-item
            class="d-flex justify-content-between align-items-center"
          >
            Cras justo odio
            <b-badge variant="primary" pill>14</b-badge>
          </b-list-group-item>

          <b-list-group-item
            class="d-flex justify-content-between align-items-center"
          >
            Dapibus ac facilisis in
            <b-badge variant="primary" pill>2</b-badge>
          </b-list-group-item>

          <b-list-group-item
            class="d-flex justify-content-between align-items-center"
          >
            Morbi leo risus
            <b-badge variant="primary" pill>1</b-badge>
          </b-list-group-item>
        </b-list-group>
      </b-col>
      <b-col cols="9" sm="9" md="9" lg="9" xl="9">
        <b-row>
          <b-col v-for="i in 6" :key="i" cols="12" sm="4" md="4" lg="4" xl="4">
            <SmallCard />
          </b-col>
        </b-row>
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

<style scoped>
.custom-list-gropu .list-group-item {
  cursor: pointer;
}
</style>
