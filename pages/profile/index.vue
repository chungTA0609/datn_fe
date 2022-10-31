<template>
  <section class="container container--fluid" id="dashboard">
    <div class="row">
      <div class="col-lg col-12">
        <div
          class="v-card--material pa-3 v-card--material-chart v-card v-sheet theme--light v-card--material--has-heading"
          hover-reveal=""
        >
          <div class="d-flex grow flex-wrap"></div>
          <h4 class="card-title font-weight-light mt-2 ml-2">
            Personal Information
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
            Work Information
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
            Contact Information
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
</template>

<script>
export default {
  name: 'UserProfile',
  layout: 'default',
};
</script>

<style></style>
