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
                            >Employee ID</label
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
                            >Work Email</label
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
                      :labelText="'Join Date'"
                    />
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
                            >Tax Number</label
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
                            >T??? l??? ????ng BHXH</label
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
                      :labelText="'Ng??y tham gia BHXH'"
                    />
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
                            >S??? BHYT</label
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
                            >N??i ????ng k?? kh??m BHYT</label
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
                      :labelText="'Ng??y k???t th??c ??K kh??m'"
                    />
                  </div>
                </div>
                <div class="col-md-4 col-12" style="top: -16px">
                  <div
                    class="v-input purple-input theme--light v-text-field v-text-field--is-booted"
                    :class="[isInputting ? '' : 'v-input--is-disabled']"
                  >
                    <DatePicker
                      :isInputting="isInputting"
                      :labelText="'Last employed date'"
                    />
                  </div>
                </div>
                <div class="col col-12">
                  <div
                    class="v-input v-textarea v-input--is-dirty theme--light v-text-field v-text-field--is-booted"
                    :class="[
                      isInputting
                        ? 'v-input--is-label-active'
                        : 'v-input--is-disabled',
                    ]"
                  >
                    <div class="v-input__control">
                      <div class="v-input__slot">
                        <div class="v-text-field__slot">
                          <label
                            for="input-222"
                            class="v-label v-label--active theme--light"
                            style="left: 0px; right: auto; position: absolute"
                            >Reasons for leaving the job</label
                          ><textarea id="input-222" rows="5"></textarea>
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
              Rick Owens??? bed design but the back is...
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
  name: 'WorkInfo',
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
