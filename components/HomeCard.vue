<template>
  <div class="pb-3">
    <nuxt-link to="/hello">
      <b-row no-gutters>
        <b-col cols="6" sm="6" md="6" lg="6" xl="6">
          <b-card
            no-body
            img-alt="card-picture"
            img-height="200"
            img-src="~/assets/cover-one.png"
          >
          </b-card>
        </b-col>
        <b-col cols="6" sm="6" md="6" class="my-auto" lg="6" xl="6">
          <div class="custom-card-text pl-2">
            <div class="title">
              <h5>
                <strong>{{ article.post_title }}</strong>
              </h5>
            </div>
            <div class="pt-2">
              <p>
                {{ article.post_description }}
              </p>
            </div>
          </div>
        </b-col>
      </b-row>
    </nuxt-link>
  </div>
</template>

<script>
export default {
  name: 'HomeCard',
  props: {
    // eslint-disable-next-line vue/require-default-prop
    article: {
      type: Object,
    },
  },
}
</script>

<style></style>
