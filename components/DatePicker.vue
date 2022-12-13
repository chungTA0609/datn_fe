<template>
  <v-row>
    <v-col>
      <v-menu
        ref="menu"
        v-model="menu"
        :close-on-content-click="false"
        :return-value.sync="dateTime"
        transition="scale-transition"
        offset-y
        min-width="auto"
      >
        <template v-slot:activator="{ on, attrs }">
          <v-text-field
            v-model="dateTime"
            :label="labelText"
            prepend-icon="mdi-calendar"
            :disabled="!isInputting"
            v-bind="attrs"
            v-on="on"
          ></v-text-field>
        </template>
        <v-date-picker v-model="date" no-title scrollable>
          <v-spacer></v-spacer>
          <v-btn text color="primary" @click="menu = false"> Cancel </v-btn>
          <v-btn text color="primary" @click="confirmDate"> OK </v-btn>
        </v-date-picker>
      </v-menu>
    </v-col>
  </v-row>
</template>
<script>
export default {
  name: 'DatePicker',
  props: {
    isInputting: {
      type: Boolean,
      default: false,
    },
    labelText: {
      type: String,
      default: '',
    },
    dateTime: {
      type: String,
      default: '',
    },
  },
  data: () => ({
    date: new Date(Date.now() - new Date().getTimezoneOffset() * 60000)
      .toISOString()
      .substr(0, 10),
    menu: false,
    modal: false,
    menu2: false,
  }),
  methods: {
    confirmDate() {
      this.$refs.menu.save(this.dateTime);
      this.$emit('update:dateTime', this.dateTime);
    },
  },
};
</script>
