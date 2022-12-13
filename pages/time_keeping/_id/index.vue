<template>
  <section class="container container--fluid" id="regular-tables">
    <section class="mb-12 text-center">
      <h1 class="font-weight-light mb-2 headline">
        Timekeeping month 12 year 2022
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
          <div class="card-title font-weight-light">
            Total paid working days: {{ sumAmount }}/{{ DATA.length }}
          </div>
        </div>
      </div>
      <div class="v-data-table theme--light">
        <div class="v-data-table__wrapper">
          <table>
            <thead>
              <tr>
                <th
                  v-for="(item, idx) in LABEL"
                  :key="idx"
                  class="primary--text"
                >
                  {{ item.name }}
                </th>
              </tr>
            </thead>
            <tbody>
              <tr v-for="(item, idx) in DATA" :key="idx">
                <td>{{ item.date }}</td>
                <td>{{ item.time_in_morning }}</td>
                <td>{{ item.time_out_morning }}</td>
                <td>{{ item.time_in_afternoon }}</td>
                <td>{{ item.time_out_morning }}</td>
                <td>{{ item.amount }}</td>
                <td>{{ item.type }}</td>
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
import { LABEL, DATA } from '~/constants/time_keeping';
export default {
  name: 'TableTimeKeeping',
  data() {
    return { LABEL, DATA, sumAmount: 0 };
  },
  mounted() {
    this.sumAmount = this.DATA.reduce((sum, a) => sum + a.amount, 0);
  },
};
</script>

<style></style>
