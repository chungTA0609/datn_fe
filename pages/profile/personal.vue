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
              <div class="display-2 font-weight-light">Edit Profile</div>
              <div class="subtitle-1 font-weight-light">
                Complete your profile
              </div>
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
                            class="v-label theme--light"
                            :class="[isInputting ? '' : 'v-label--is-disabled']"
                            style="left: 0px; right: auto; position: absolute"
                            >Company</label
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
                <div class="col-md-4 col-12" style="top: -16px">
                  <div
                    class="v-input theme--light v-text-field v-text-field--is-booted"
                    :class="[isInputting ? '' : 'v-input--is-disabled']"
                  >
                    <v-select
                      :items="items"
                      label="Gender"
                      :disabled="!isInputting"
                    ></v-select>
                  </div>
                </div>
                <div class="col-md-4 col-12" style="top: -16px">
                  <div
                    class="v-input purple-input theme--light v-text-field v-text-field--is-booted"
                    :class="[isInputting ? '' : 'v-input--is-disabled']"
                  >
                    <DatePicker
                      :isInputting="isInputting"
                      :labelText="'Date of Birth'"
                    />
                  </div>
                </div>
                <div class="col-md-6 col-12">
                  <div
                    class="v-input purple-input theme--light v-text-field v-text-field--is-booted"
                    :class="[isInputting ? '' : 'v-input--is-disabled']"
                  >
                    <div class="v-input__control">
                      <div class="v-input__slot">
                        <div class="v-text-field__slot">
                          <label
                            for="input-204"
                            class="v-label theme--light"
                            :class="[isInputting ? '' : 'v-label--is-disabled']"
                            style="left: 0px; right: auto; position: absolute"
                            >First Name</label
                          ><input
                            :disabled="!isInputting"
                            id="input-204"
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
                <div class="col-md-6 col-12">
                  <div
                    class="v-input purple-input theme--light v-text-field v-text-field--is-booted"
                    :class="[isInputting ? '' : 'v-input--is-disabled']"
                  >
                    <div class="v-input__control">
                      <div class="v-input__slot">
                        <div class="v-text-field__slot">
                          <label
                            for="input-207"
                            class="v-label theme--light"
                            :class="[isInputting ? '' : 'v-label--is-disabled']"
                            style="left: 0px; right: auto; position: absolute"
                            >Last Name</label
                          ><input
                            :disabled="!isInputting"
                            id="input-207"
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
                            class="v-label theme--light"
                            :class="[isInputting ? '' : 'v-label--is-disabled']"
                            style="left: 0px; right: auto; position: absolute"
                            >CCCD</label
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
                            class="v-label theme--light"
                            :class="[isInputting ? '' : 'v-label--is-disabled']"
                            style="left: 0px; right: auto; position: absolute"
                            >Nơi cấp</label
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
                <div class="col-md-4 col-12" style="top: -16px">
                  <div
                    class="v-input purple-input theme--light v-text-field v-text-field--is-booted"
                    :class="[isInputting ? '' : 'v-input--is-disabled']"
                  >
                    <DatePicker
                      :isInputting="isInputting"
                      :labelText="'Ngày cấp'"
                    />
                  </div>
                </div>
                <div class="col-md-6 col-12" style="top: -16px">
                  <div
                    class="v-input purple-input theme--light v-text-field v-text-field--is-booted"
                    :class="[isInputting ? '' : 'v-input--is-disabled']"
                  >
                    <v-select
                      :items="items"
                      label="Tôn giáo"
                      :disabled="!isInputting"
                    ></v-select>
                  </div>
                </div>
                <div class="col-md-6 col-12" style="top: -16px">
                  <div
                    class="v-input purple-input theme--light v-text-field v-text-field--is-booted"
                    :class="[isInputting ? '' : 'v-input--is-disabled']"
                  >
                    <v-select
                      :items="items"
                      label="Dân tộc"
                      :disabled="!isInputting"
                    ></v-select>
                  </div>
                </div>
                <div class="col-md-6 col-12" style="top: -16px">
                  <div
                    class="v-input purple-input theme--light v-text-field v-text-field--is-booted"
                    :class="[isInputting ? '' : 'v-input--is-disabled']"
                  >
                    <v-select
                      :items="items"
                      label="Tình trạng hôn nhân"
                      :disabled="!isInputting"
                    ></v-select>
                  </div>
                </div>
                <div class="col-md-6 col-12" style="top: -16px">
                  <div
                    class="v-input purple-input theme--light v-text-field v-text-field--is-booted"
                    :class="[isInputting ? '' : 'v-input--is-disabled']"
                  >
                    <v-select
                      :items="items"
                      label="Quốc tịch"
                      :disabled="!isInputting"
                    ></v-select>
                  </div>
                </div>
              </div>
              <div class="text-right col col-12">
                <button
                  type="button"
                  class="mr-0 v-btn v-btn--contained theme--light v-size--default"
                  @click="handleOnEdit"
                >
                  <span class="v-btn__content"> Edit Profile </span>
                </button>
                <button
                  v-if="isInputting"
                  type="button"
                  class="mr-0 v-btn v-btn--contained theme--light v-size--default"
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
      <div class="col-md-4 col-12">
        <div
          class="v-card--material pa-3 v-card-profile v-card v-sheet theme--light"
        >
          <div class="d-flex grow flex-wrap">
            <div
              class="v-avatar mx-auto v-card--material__avatar elevation-6 grey"
              style="height: 128px; min-width: 128px; width: 128px"
            >
              <div class="v-responsive v-image">
                <div
                  class="v-responsive__sizer"
                  style="padding-bottom: 100%"
                ></div>
                <div
                  class="v-image__image v-image__image--cover"
                  style="
                    background-image: url('https://demos.creative-tim.com/vue-material-dashboard/img/marc.aba54d65.jpg');
                    background-position: center center;
                  "
                ></div>
                <div class="v-responsive__content" style="width: 400px"></div>
              </div>
            </div>
            <!---->
          </div>
          <div class="v-card__text text-center">
            <h6 class="display-1 mb-1 grey--text">CEO / CO-FOUNDER</h6>
            <h4 class="display-2 font-weight-light mb-3 black--text">
              Alec Thompson
            </h4>
            <p class="font-weight-light grey--text">
              Don't be scared of the truth because we need to restart the human
              foundation in truth And I love you like Kanye loves Kanye I love
              Rick Owens’ bed design but the back is...
            </p>
            <button
              type="button"
              class="mr-0 v-btn v-btn--contained v-btn--rounded theme--light v-size--default success"
            >
              <span class="v-btn__content"> Follow </span>
            </button>
          </div>
          <!---->
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import DatePicker from '~/components/DatePicker.vue';
export default {
  name: 'PersonalInfo',
  layout: 'default',
  components: {
    DatePicker,
  },
  data() {
    return {
      isInputting: false,
      items: ['Foo', 'Bar', 'Fizz', 'Buzz'],
    };
  },
  methods: {
    handleOnEdit() {
      this.isInputting = true;
    },
    handleOnCancel() {
      this.isInputting = false;
    },
  },
};
</script>

<style></style>
