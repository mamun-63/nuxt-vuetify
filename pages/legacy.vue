<template>
  <div class="mx-8">
    <v-switch
      v-model="$vuetify.theme.dark"
      hint="This toggles the global state of the Vuetify theme"
      inset
      label="Vuetify Theme Dark"
      persistent-hint
    />

    <v-row>
      <v-col>
        <v-card v-for="data in cardData" :key="data.title">
          <p>{{ data.title }}</p>
          <p>{{ data.date }}</p>
        </v-card>
      </v-col>
    </v-row>

    <v-row>
      <v-col cols="12" sm="6" md="4">
        <v-card>
          <div class="pa-3">
            <v-row>
              <v-col md="6">
                <p class="red--text">
                  US ELECTION
                </p>
              </v-col>
              <v-col md="6" class="d-flex flex-row-reverse">
                <p>31 OCT, 2020</p>
              </v-col>
            </v-row>
            <p class="display-1 mb-3">
              Trump’s biggest campaign promises: Did he deliver?
            </p>
            <p>With just a day of campaigning left, the two candidates rally in key states as the bitter presidential race nears an end.</p>
            <v-btn text class="red--text">
              full news
              <v-icon>mdi-export</v-icon>
            </v-btn>
          </div>
          <v-img
            height="250"
            src="https://cdn.vuetifyjs.com/images/cards/docks.jpg"
          >
            <v-row justify="center" align="center" class="mx-2">
              <v-col md="6">
                <small class="white--text">7 Minutes Read</small>
              </v-col>
              <v-col md="6" class="d-flex flex-row-reverse">
                <v-progress-linear color="red" value="67" />
              </v-col>
            </v-row>
          </v-img>
        </v-card>
      </v-col>

      <v-col cols="12" sm="6" md="4">
        <v-card>
          <div class="pa-3">
            <v-row>
              <v-col md="6">
                <p class="red--text">
                  US ELECTION
                </p>
              </v-col>
              <v-col md="6" class="d-flex flex-row-reverse">
                <p>31 OCT, 2020</p>
              </v-col>
            </v-row>
            <p class="display-1 mb-3">
              Trump’s biggest campaign promises: Did he deliver?
            </p>
            <p>With just a day of campaigning left, the two candidates rally in key states as the bitter presidential race nears an end.</p>
            <v-btn text class="red--text">
              full news
              <v-icon>mdi-export</v-icon>
            </v-btn>
          </div>
          <v-img
            height="250"
            src="https://cdn.vuetifyjs.com/images/cards/docks.jpg"
          >
            <v-row justify="center" align="center" class="mx-2">
              <v-col md="6">
                <small class="white--text">7 Minutes Read</small>
              </v-col>
              <v-col md="6" class="d-flex flex-row-reverse">
                <v-progress-linear color="red" value="67" />
              </v-col>
            </v-row>
          </v-img>
        </v-card>
      </v-col>

      <v-col cols="12" sm="6" md="4">
        <v-card>
          <div class="pa-3">
            <v-row>
              <v-col md="6">
                <p class="red--text">
                  US ELECTION
                </p>
              </v-col>
              <v-col md="6" class="d-flex flex-row-reverse">
                <p>31 OCT, 2020</p>
              </v-col>
            </v-row>
            <p class="display-1 mb-3">
              Trump’s biggest campaign promises: Did he deliver?
            </p>
            <p>With just a day of campaigning left, the two candidates rally in key states as the bitter presidential race nears an end.</p>
            <v-btn text class="red--text">
              full news
              <v-icon>mdi-export</v-icon>
            </v-btn>
          </div>
          <v-img
            height="250"
            src="https://cdn.vuetifyjs.com/images/cards/docks.jpg"
          >
            <v-row justify="center" align="center" class="mx-2">
              <v-col md="6">
                <small class="white--text">7 Minutes Read</small>
              </v-col>
              <v-col md="6" class="d-flex flex-row-reverse">
                <v-progress-linear color="red" value="67" />
              </v-col>
            </v-row>
          </v-img>
        </v-card>
      </v-col>
    </v-row>

    <v-card height="77" width="276">
      <div class="d-flex justify-space-between">
        <p>ফ্রান্স</p>
        <p>৬৭%</p>
      </div>
      <v-progress-linear color="amber" value="67" />
      <small>৪৩২৩১ ভোট</small>
    </v-card>
    <div class="d-flex justify-space-between">
      <p>Text left</p>
      <p>Text right</p>
    </div>
    <div class="d-flex justify-space-between">
      <v-btn>Button</v-btn>
      <v-btn>Button</v-btn>
    </div>
    <div class="d-flex flex-row-reverse mt-5">
      <v-btn>Right</v-btn>
    </div>
    <v-card-actions>
      <v-spacer />
      <v-btn>Right</v-btn>
    </v-card-actions>
    <v-divider class="indigo mt-5" />

    <p class="display-1">
      Display Helpers
    </p>
    <p class="hidden-sm-only">
      Visibility
    </p>
    <p class="d-block primary">
      d-block
    </p>
    <p class="d-inline primary">
      d-inline
    </p>
    <p class="d-inline primary">
      d-inline
    </p>

    <v-divider class="indigo mt-5" />

    <p class="font-italic display-1">
      Text and Typography
    </p>
    <div class="text-truncate" style="max-width: 150px;">
      Suspendisse faucibus, nunc et pellentesque egestas, lacus ante convallis tellus.
    </div>
    <p class="text-capitalized">
      Text LowErcase/ uppercase/ capitalized
    </p>
    <p class="text--disabled">
      text primary, secondary, disabled
    </p>
    <p class="text-decoration-line-through">
      text decoration/ uderline, overline, line-through, none
    </p>
    <p class="text-right">
      text-right
    </p>
    <!-- by default xs, otherwise you have to specify -->
    <p class="text-center text-md-left">
      text left for md
    </p>
    <p class="headline text-uppercase">
      Headline
    </p>
    <p class="caption">
      Caption
    </p>
    <p class="overline">
      Overline
    </p>
    <p class="body 1-2">
      Body 1 and 2
    </p>
    <p class="subtitle-2">
      subtitle 1-2
    </p>
    <p class="display-2 text-md-caption">
      Display 1-4 and for small screen its caption
    </p>
    <small>small text</small>
    <v-divider class="indigo mt-5" />

    <v-btn large text class="primary lighten-2 black--text">
      Button
    </v-btn>
    <v-row>
      <v-col cols="12" sm="6" md="6">
        <v-card outlined class="pa-md-2">
          <v-card-title>This is card</v-card-title>
        </v-card>
      </v-col>
      <v-col cols="12" sm="6" md="6">
        <v-card outlined>
          <v-card-title>This is card</v-card-title>
        </v-card>
      </v-col>
    </v-row>
    <div class="pa-md-10 d-flex justify-md-end">
      <p>Hey Bro</p>
      <p>Whats up!</p>
    </div>
    <div class="d-flex flex-md-column flex-sm-row align-end">
      <p>Hey Bro</p>
      <p>Whats up!</p>
    </div>
    <div class="d-flex flex-row-reverse">
      <p>Text1</p>
      <p>Text2</p>
    </div>
    <v-row>
      <v-col class="d-flex flex-row-reverse">
        <p>This is a simple paragraph</p>
        <p>This is a another paragraph</p>
        <v-btn>Button</v-btn>
      </v-col>
    </v-row>
    <v-row>
      <v-col class="d-flex flex-row">
        <p>This is a simple paragraph</p>
        <p>This is a another paragraph</p>
        <v-btn>Button</v-btn>
      </v-col>
    </v-row>
    <v-card class="d-flex justify-space-around">
      <p>Hello</p>
      <p>Hey</p>
    </v-card>
  </div>
</template>

<script>
export default {
  data () {
    return {
      cardData: [
        { title: 'US ELECTION' },
        { date: '13 Oct, 2020' },
        { heading: 'Trump’s biggest campaign promises: Did he deliver?' },
        { description: 'With just a day of campaigning left, the two candidates rally in key states as the bitter presidential race nears an end.' },
        { src: 'https://cdn.vuetifyjs.com/images/cards/docks.jpg' }
      ]
    }
  }
}
</script>
