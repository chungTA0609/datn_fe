<template>
  <section class="container container--fluid" id="user-profile">
    <div class="row justify-center">
      <div class="col-md-8 col-12">
        <div
          class="v-card--material pa-3 v-card v-sheet theme--light v-card--material--has-heading"
        >
          <div class="d-flex grow flex-wrap">
            <div
              class="text-start v-card--material__heading mb-n6 v-sheet theme--dark elevation-6 pa-7"
              style="width: 100%; background-color: #8d448b; border-radius: 4px"
            >
              <div class="display-2 font-weight-light">
                Details of adding missing attendance
              </div>
              <div class="subtitle-1 font-weight-light"></div>
              <!---->
            </div>
            <!---->
          </div>
          <form novalidate="novalidate" class="v-form">
            <div class="container py-0">
              <div class="row">
                <div class="col-md-4 col-12">
                  <div
                    class="v-input theme--light v-text-field v-text-field--is-booted"
                    :class="[isInputting ? '' : 'v-input--is-disabled']"
                  >
                    <div class="v-input__control">
                      <div class="v-input__slot">
                        <div class="v-text-field__slot">
                          <label
                            for="input-195"
                            class="v-label v-label--active theme--light"
                            :class="[isInputting ? '' : 'v-label--is-disabled']"
                            style="left: 0px; right: auto; position: absolute"
                            >Name</label
                          ><input
                            :disabled="!isInputting"
                            id="input-195"
                            type="text"
                          />
                        </div>
                      </div>
                      <div class="v-text-field__details">
                        <div class="v-messages theme--light">
                          <div class="v-messages__wrapper"></div>
                        </div>
                      </div>
                    </div>
                  </div>
                </div>
                <div class="col-md-4 col-12">
                  <div
                    class="v-input theme--light v-text-field v-text-field--is-booted"
                    :class="[isInputting ? '' : 'v-input--is-disabled']"
                  >
                    <div class="v-input__control">
                      <div class="v-input__slot">
                        <div class="v-text-field__slot">
                          <label
                            for="input-195"
                            class="v-label v-label--active theme--light"
                            :class="[isInputting ? '' : 'v-label--is-disabled']"
                            style="left: 0px; right: auto; position: absolute"
                            >ID</label
                          ><input
                            :disabled="!isInputting"
                            id="input-196"
                            type="text"
                          />
                        </div>
                      </div>
                      <div class="v-text-field__details">
                        <div class="v-messages theme--light">
                          <div class="v-messages__wrapper"></div>
                        </div>
                      </div>
                    </div>
                  </div>
                </div>
                <div class="col-md-4 col-12">
                  <div
                    class="v-input purple-input theme--light v-text-field v-text-field--is-booted"
                    :class="[isInputting ? '' : 'v-input--is-disabled']"
                  >
                    <div class="v-input__control">
                      <div class="v-input__slot">
                        <div class="v-text-field__slot">
                          <label
                            for="input-195"
                            class="v-label v-label--active theme--light"
                            :class="[isInputting ? '' : 'v-label--is-disabled']"
                            style="left: 0px; right: auto; position: absolute"
                            >Position</label
                          ><input disabled id="input-195" type="text" />
                        </div>
                      </div>
                      <div class="v-text-field__details">
                        <div class="v-messages theme--light">
                          <div class="v-messages__wrapper"></div>
                        </div>
                      </div>
                    </div>
                  </div>
                </div>
                <div class="col-md-4 col-12">
                  <div
                    class="v-input purple-input theme--light v-text-field v-text-field--is-booted"
                    :class="[isInputting ? '' : 'v-input--is-disabled']"
                  >
                    <div class="v-input__control">
                      <div class="v-input__slot">
                        <div class="v-text-field__slot">
                          <label
                            for="input-204"
                            class="v-label v-label--active theme--light"
                            :class="[isInputting ? '' : 'v-label--is-disabled']"
                            style="left: 0px; right: auto; position: absolute"
                            >Approver</label
                          ><input
                            :disabled="!isInputting"
                            id="input-204"
                            type="text"
                            v-model="formData.approver"
                          />
                        </div>
                      </div>
                      <div class="v-text-field__details">
                        <div class="v-messages theme--light">
                          <div class="v-messages__wrapper"></div>
                        </div>
                      </div>
                    </div>
                  </div>
                </div>
                <div class="col-md-4 col-12">
                  <div
                    class="v-input purple-input theme--light v-text-field v-text-field--is-booted"
                    :class="[isInputting ? '' : 'v-input--is-disabled']"
                  >
                    <div class="v-input__control">
                      <div class="v-input__slot">
                        <div class="v-text-field__slot">
                          <label
                            for="input-207"
                            class="v-label v-label--active theme--light"
                            :class="[isInputting ? '' : 'v-label--is-disabled']"
                            style="left: 0px; right: auto; position: absolute"
                            >Related person</label
                          ><input
                            :disabled="!isInputting"
                            id="input-207"
                            type="text"
                            v-model="formData.relatedPerson"
                          />
                        </div>
                      </div>
                      <div class="v-text-field__details">
                        <div class="v-messages theme--light">
                          <div class="v-messages__wrapper"></div>
                        </div>
                      </div>
                    </div>
                  </div>
                </div>
                <div class="col-md-1 col-12" style="padding-top: 20px">
                  <div class="col col-4">
                    <div class="v-list-item__action">
                      <div
                        class="v-input theme--light v-input--selection-controls v-input--checkbox"
                        :class="[
                          formData.isOT
                            ? 'secondary--text v-input--is-label-active v-input--is-dirty'
                            : '',
                          isInputting ? '' : 'v-input--is-disabled',
                        ]"
                      >
                        <div class="v-input__control" @click="changeIsOT">
                          <div class="v-input__slot">
                            <div class="v-input--selection-controls__input">
                              <i
                                aria-hidden="true"
                                class="v-icon notranslate mdi theme--light"
                                :class="[
                                  formData.isOT
                                    ? 'secondary--text mdi-checkbox-marked'
                                    : 'mdi-checkbox-blank-outline',
                                ]"
                              ></i
                              ><input
                                :aria-checked="formData.isOT"
                                id="input-1073"
                                role="checkbox"
                                type="checkbox"
                              />
                              <div
                                class="v-input--selection-controls__ripple"
                                :class="[
                                  formData.isOT
                                    ? 'secondary--text'
                                    : 'primary--text',
                                ]"
                              ></div>
                            </div>
                          </div>
                          <div
                            class="v-messages theme--light"
                            :class="[formData.isOT ? 'secondary--text' : '']"
                          >
                            <div class="v-messages__wrapper"></div>
                          </div>
                        </div>
                      </div>
                    </div>
                  </div>
                </div>
                <div class="col-md-3 col-12" style="padding-top: 30px">
                  <div class="col col-12">
                    <div class="font-weight-light">Adding Missing OT hours</div>
                  </div>
                </div>
                <div class="col-md-6 col-12" style="top: -16px">
                  <div
                    class="v-input purple-input theme--light v-text-field v-text-field--is-booted"
                    :class="[isInputting ? '' : 'v-input--is-disabled']"
                  >
                    <DatePicker
                      :isInputting="isInputting"
                      :labelText="'Start date'"
                      :dateTime.sync="formData.startDate"
                    />
                  </div>
                </div>
                <div class="col-md-6 col-12" style="top: -16px">
                  <div
                    class="v-input purple-input theme--light v-text-field v-text-field--is-booted"
                    :class="[isInputting ? '' : 'v-input--is-disabled']"
                  >
                    <DatePicker
                      :isInputting="isInputting"
                      :labelText="'End date'"
                      :dateTime.sync="formData.endDate"
                    />
                  </div>
                </div>
                <div class="col col-12">
                  <div
                    class="v-input purple-input v-textarea v-input--is-label-active v-input--is-dirty theme--light v-text-field v-text-field--is-booted"
                    :class="[isInputting ? '' : 'v-input--is-disabled']"
                  >
                    <div class="v-input__control">
                      <div class="v-input__slot">
                        <div class="v-text-field__slot">
                          <label
                            for="input-3182"
                            class="v-label v-label--active theme--light"
                            style="left: 0px; right: auto; position: absolute"
                            >Reason</label
                          ><textarea id="input-3182" rows="5"></textarea>
                        </div>
                      </div>
                      <div class="v-text-field__details">
                        <div class="v-messages theme--light">
                          <div class="v-messages__wrapper"></div>
                        </div>
                      </div>
                    </div>
                  </div>
                </div>
              </div>
              <div class="text-right col col-12">
                <button
                  type="button"
                  class="mr-0 v-btn v-btn--contained theme--dark v-size--default"
                  @click="handleOnEdit"
                >
                  <span class="v-btn__content"> Edit Profile </span>
                </button>
                <button
                  v-if="isInputting"
                  type="button"
                  class="mr-0 v-btn v-btn--contained theme--gray v-size--default"
                  @click="handleOnCancel"
                >
                  <span class="v-btn__content"> Cancel </span>
                </button>
              </div>
            </div>
          </form>
          <!---->
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import DatePicker from '~/components/DatePicker.vue';
export default {
  name: 'DetailsMissingTicket',
  components: {
    DatePicker,
  },
  data() {
    return {
      isInputting: false,
      items: ['Foo', 'Bar', 'Fizz', 'Buzz'],
      formData: {
        approver: null,
        isOT: false,
        relatedPerson: null,
        startDate: null,
        endDate: null,
        reason: '',
      },
    };
  },
  mounted() {
    this.formData.startDate = new Date(
      Date.now() - new Date().getTimezoneOffset() * 60000
    )
      .toISOString()
      .substr(0, 10);
    this.formData.endDate = new Date(
      Date.now() - new Date().getTimezoneOffset() * 60000
    )
      .toISOString()
      .substr(0, 10);
  },
  methods: {
    handleOnEdit() {
      this.isInputting = true;
    },
    handleOnCancel() {
      this.isInputting = false;
    },
    changeIsOT() {
      this.formData.isOT = !this.formData.isOT;
    },
  },
};
</script>

<style></style>
