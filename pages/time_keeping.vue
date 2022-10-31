<template>
  <div class="v-content__wrap">
    <section class="container container--fluid" id="dashboard">
      <div class="row">
        <div class="col-lg col-12">
          <div
            class="v-card--material pa-3 v-card--material-chart v-card v-sheet theme--light v-card--material--has-heading"
            hover-reveal=""
          >
            <div class="d-flex grow flex-wrap"></div>
            <h4 class="card-title font-weight-light mt-2 ml-2">
              Website Views
            </h4>
            <p class="d-inline-flex font-weight-light ml-2 mt-1">
              Last Campaign Performance
            </p>
            <hr
              role="separator"
              aria-orientation="horizontal"
              class="mt-2 v-divider theme--light"
            />
            <div class="v-card__actions pb-0">
              <i
                aria-hidden="true"
                class="v-icon notranslate mr-1 mdi mdi-clock-outline theme--light"
                style="font-size: 16px"
              ></i
              ><span class="caption grey--text font-weight-light"
                >updated 10 minutes ago</span
              >
            </div>
          </div>
        </div>
      </div>
      <div class="row">
        <div class="col-lg col-12">
          <div
            class="v-card--material pa-3 v-card--material-chart v-card v-sheet theme--light v-card--material--has-heading"
            hover-reveal=""
          >
            <div class="d-flex grow flex-wrap"></div>
            <h4 class="card-title font-weight-light mt-2 ml-2">
              Website Views
            </h4>
            <p class="d-inline-flex font-weight-light ml-2 mt-1">
              Last Campaign Performance
            </p>
            <hr
              role="separator"
              aria-orientation="horizontal"
              class="mt-2 v-divider theme--light"
            />
            <div class="v-card__actions pb-0">
              <i
                aria-hidden="true"
                class="v-icon notranslate mr-1 mdi mdi-clock-outline theme--light"
                style="font-size: 16px"
              ></i
              ><span class="caption grey--text font-weight-light"
                >updated 10 minutes ago</span
              >
            </div>
          </div>
        </div>
      </div>
      <div class="row">
        <div class="col-lg col-12">
          <div
            class="v-card--material pa-3 v-card--material-chart v-card v-sheet theme--light v-card--material--has-heading"
            hover-reveal=""
          >
            <div class="d-flex grow flex-wrap"></div>
            <h4 class="card-title font-weight-light mt-2 ml-2">
              Website Views
            </h4>
            <p class="d-inline-flex font-weight-light ml-2 mt-1">
              Last Campaign Performance
            </p>
            <hr
              role="separator"
              aria-orientation="horizontal"
              class="mt-2 v-divider theme--light"
            />
            <div class="v-card__actions pb-0">
              <i
                aria-hidden="true"
                class="v-icon notranslate mr-1 mdi mdi-clock-outline theme--light"
                style="font-size: 16px"
              ></i
              ><span class="caption grey--text font-weight-light"
                >updated 10 minutes ago</span
              >
            </div>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
import Square from '~/components/Square.vue';
export default {
  name: 'TimeKeeping',
  layout: 'default',
  components: {
    Square,
  },
};
</script>

<style>
.ct-square {
  max-height: 150px;
}
</style>
