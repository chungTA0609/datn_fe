<template>
  <section class="container container--fluid" id="regular-tables">
    <section class="mb-12 text-center">
      <h1 class="font-weight-light mb-2 headline">
        Paid leave tickets related to me
      </h1>
    </section>
    <div
      class="v-card--material pa-3 px-5 py-3 v-card v-sheet theme--light v-card--material--has-heading"
    >
      <div class="d-flex grow flex-wrap">
        <div
          class="text-start v-card--material__heading mb-n6 v-sheet theme--dark elevation-6 success pa-7"
          style="max-height: 90px; width: auto"
        >
          <i
            aria-hidden="true"
            class="v-icon notranslate mdi mdi-clipboard-text theme--dark"
            style="font-size: 32px"
          ></i
          ><!---->
        </div>
        <div class="ml-4">
          <div class="card-title font-weight-light"></div>
        </div>
      </div>
      <div class="v-data-table theme--light">
        <div class="v-data-table__wrapper">
          <table>
            <thead>
              <tr>
                <th
                  v-for="(item, idx) in LIST_LABEL"
                  :key="idx"
                  class="primary--text"
                >
                  {{ item.name }}
                </th>
              </tr>
            </thead>
            <tbody>
              <tr v-for="(item, idx) in LIST_DATA" :key="idx">
                <td>{{ item.month }}</td>
                <td>{{ item.start_date }}</td>
                <td>{{ item.end_date }}</td>
                <td>{{ item.registration_date }}</td>
                <td>{{ item.approval_time }}</td>
                <td>{{ item.amount }}</td>
                <td>{{ item.type }}</td>
                <td>{{ item.reason }}</td>
                <td>{{ item.status }}</td>
                <td>
                  <a
                    ><div
                      class="text-start mb-n0 v-sheet theme--dark green pa-1 v-btn"
                      style="max-height: 50px; width: 35px; border-radius: 10px"
                      @click="gotoUrl('/paid_leave/details/' + item.id)"
                    >
                      <i
                        aria-hidden="true"
                        class="v-icon notranslate mdi mdi-alert-circle theme--dark"
                        style="font-size: 20px; position: relative"
                      ></i
                      ><!---->
                    </div></a
                  >
                </td>
              </tr>
            </tbody>
          </table>
        </div>
      </div>
      <!---->
    </div>
  </section>
</template>

<script>
import { LIST_LABEL, LIST_DATA } from '~/constants/paid_leave';
import url from '~/mixins/url';
export default {
  name: 'RelateMePaid',
  mixins: [url],
  data() {
    return { LIST_LABEL, LIST_DATA, sumAmount: 0 };
  },
  mounted() {
    console.log(this.$route.path.spli);
    // this.sumAmount = this.DATA.reduce((sum, a) => sum + a.amount, 0);
  },
};
</script>

<style></style>
