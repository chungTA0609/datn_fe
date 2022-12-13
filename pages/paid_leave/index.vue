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
              <a
                ><span @click="gotoUrl($route.path + '/my_ticket')"
                  >My paid leave registrations</span
                ></a
              >
            </h4>
            <p class="d-inline-flex font-weight-light ml-2 mt-1"></p>
            <hr
              role="separator"
              aria-orientation="horizontal"
              class="mt-2 v-divider theme--light"
            />
            <div class="v-card__actions pb-0">
              <span class="caption grey--text font-weight-light"></span>
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
              <a
                ><span @click="gotoUrl($route.path + '/new_ticket')"
                  >Create new Paid Ticket</span
                ></a
              >
            </h4>
            <p class="d-inline-flex font-weight-light ml-2 mt-1"></p>
            <hr
              role="separator"
              aria-orientation="horizontal"
              class="mt-2 v-divider theme--light"
            />
            <div class="v-card__actions pb-0">
              <span class="caption grey--text font-weight-light"></span>
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
              <a
                ><span @click="gotoUrl($route.path + '/relate_me')"
                  >Paid leave registrations related to me</span
                ></a
              >
            </h4>
            <p class="d-inline-flex font-weight-light ml-2 mt-1"></p>
            <hr
              role="separator"
              aria-orientation="horizontal"
              class="mt-2 v-divider theme--light"
            />
            <div class="v-card__actions pb-0">
              <span class="caption grey--text font-weight-light"></span>
            </div>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
import Square from '~/components/Square.vue';
import url from '~/mixins/url';
export default {
  name: 'PaidLeave',
  mixins: [url],
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
