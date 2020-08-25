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
                <strong>This is a title of our beautiful blog</strong>
              </h5>
            </div>
            <div class="pt-2">
              <p>
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Et est
                quos officia po. Lorem ipsum dolor sit amet consectetur..
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
}
</script>

<style></style>
