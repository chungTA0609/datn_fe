<template>
  <div
    data-app="true"
    class="v-application v-application--is-ltr theme--light"
    id="app"
  >
    <div class="v-application--wrap">
      <nav
        class="v-navigation-drawer v-navigation-drawer--fixed v-navigation-drawer--open theme--dark"
        id="core-navigation-drawer"
        data-booted="true"
      >
        <div class="v-navigation-drawer__image">
          <div class="v-responsive v-image">
            <div
              class="v-image__image v-image__image--preload v-image__image--cover"
            ></div>
            <div class="v-responsive__content"></div>
          </div>
          <div class="v-responsive v-image">
            <div
              class="v-image__image v-image__image--preload v-image__image--cover"
            ></div>
            <div class="v-responsive__content"></div>
          </div>
        </div>
        <div class="v-navigation-drawer__content">
          <hr
            role="separator"
            aria-orientation="horizontal"
            class="mb-1 v-divider theme--dark"
          />
          <div
            class="v-list v-sheet v-sheet--tile theme--dark v-list--dense v-list--nav"
          >
            <div tabindex="-1" class="v-list-item theme--dark">
              <div
                class="v-avatar v-list-item__avatar align-self-center white"
                contain=""
                style="height: 40px; min-width: 40px; width: 40px"
              >
                <div class="v-responsive v-image" style="max-height: 30px">
                  <div
                    class="v-responsive__sizer"
                    style="padding-bottom: 100%"
                  ></div>
                  <div
                    class="v-image__image v-image__image--cover"
                    style="
                      background-image: url(urlImage);
                      background-position: center center;
                    "
                  ></div>
                  <div class="v-responsive__content"></div>
                </div>
              </div>
              <div class="v-list-item__content">
                <div class="v-list-item__title">Vuetify MD</div>
              </div>
            </div>
          </div>
          <hr
            role="separator"
            aria-orientation="horizontal"
            class="mb-2 v-divider theme--dark"
          />
          <div class="v-list v-sheet v-sheet--tile theme--dark v-list--nav">
            <div></div>
            <a
              v-for="(item, idx) in SIDE_BAR"
              :key="idx"
              :href="item.url"
              class="v-list-item v-list-item--link theme--dark"
              :tabindex="item.id"
              ><div class="v-list-item__icon">
                <i
                  aria-hidden="true"
                  class="v-icon notranslate mdi mdi-view-dashboard theme--dark"
                ></i>
              </div>
              <div class="v-list-item__content">
                <div class="v-list-item__title">{{ item.name }}</div>
                <div class="v-list-item__subtitle"></div></div
            ></a>
            <div></div>
          </div>
        </div>
        <div class="v-navigation-drawer__append">
          <!-- <a
            href="#"
            class="v-list-item v-list-item--link theme--dark"
            tabindex="0"
            ><div class="v-list-item__icon">
              <i
                aria-hidden="true"
                class="v-icon notranslate mdi mdi-package-up theme--dark"
              ></i>
            </div>
            <div class="v-list-item__content">
              <div class="v-list-item__title"></div>
              <div class="v-list-item__subtitle"></div></div
          ></a> -->
        </div>
        <div class="v-navigation-drawer__border"></div>
      </nav>
      <main
        class="v-content"
        data-booted="true"
        style="padding: 75px 0px 0px 260px"
      >
        <div class="v-content__wrap">
          <Nuxt /><!-- <footer
          class="v-footer v-sheet v-sheet--tile theme--light"
          id="dashboard-core-footer"
          data-booted="true"
        >
          <div class="container">
            <div class="row no-gutters align-center">
              <div class="text-center mb-sm-0 mb-5 col col-auto">
                <a
                  href="#"
                  rel="noopener"
                  target="_blank"
                  class="mr-0 grey--text text--darken-3"
                  >Creative Tim</a
                >
              </div>
              <div class="text-center mb-sm-0 mb-5 col col-auto">
                <a
                  href="#"
                  rel="noopener"
                  target="_blank"
                  class="mr-0 grey--text text--darken-3"
                  >About Us</a
                >
              </div>
              <div class="text-center mb-sm-0 mb-5 col col-auto">
                <a
                  href="#"
                  rel="noopener"
                  target="_blank"
                  class="mr-0 grey--text text--darken-3"
                  >Blog</a
                >
              </div>
              <div class="text-center mb-sm-0 mb-5 col col-auto">
                <a
                  href="#"
                  rel="noopener"
                  target="_blank"
                  class="mr-0 grey--text text--darken-3"
                  >Licenses</a
                >
              </div>
              <div class="spacer hidden-sm-and-down"></div>
              <div class="col-md-auto col-12">
                <div class="body-1 font-weight-light pt-6 pt-md-0 text-center">
                  © 2019, made with
                  <i
                    aria-hidden="true"
                    class="v-icon notranslate mdi mdi-heart theme--light"
                    style="font-size: 18px"
                  ></i>
                  by <a href="https://www.creative-tim.com">Creative Tim</a> for
                  a better web.
                </div>
              </div>
            </div>
          </div>
        </footer> -->
        </div>
      </main>
    </div>
  </div>
</template>

<script>
import { SIDE_BAR } from '~/constants/sidebar';
export default {
  name: 'DefaultLayout',
  data() {
    return {
      SIDE_BAR,
      urlImage: '',
      host: '',
    };
  },
  mounted() {
    this.host = window.location.host;
  },
};
</script>

<style>
#settings {
  min-width: 100px;
  background-color: rgba(0, 0, 0, 0.3);
  border-color: rgba(0, 0, 0, 0.3);
  position: fixed;
  top: 115px;
  right: -35px;
  border-radius: 8px;
}
#core-navigation-drawer {
  height: 100vh;
  top: 0px;
  max-height: calc(100% - 0px);
  transform: translateX(0%);
  width: 260px;
  background-color: #8d448b;
}
/* .v-image__image--preload {
    background-image: linear-gradient(rgba(0, 0, 0, 0.8), rgba(0, 0, 0, 0.8));
    background-position: center center;
  } */
</style>
