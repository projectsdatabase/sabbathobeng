<template>
  <q-page class="flex flex-center">
    <div>
      <q-carousel
        class="myCarousel"
        animated
        v-model="slide"
        navigation
        infinite
        :autoplay="autoplay"
        arrows
        transition-prev="slide-right"
        transition-next="slide-left"
        @mouseenter="autoplay = false"
        @mouseleave="autoplay = true"
      >
        <q-carousel-slide
          :name="1"
          img-src="~assets/bgCarousel.jpg"
          class="myImage"
        >
          <div class="absolute-center second-caption q-mr-xl">
            <div class="text-h2 text-center">MAY SALE</div>
            <div class="text-h5 text-center text-primary">
              Up to 50% Discount
            </div>
          </div>
        </q-carousel-slide>
        <q-carousel-slide :name="2" img-src="~assets/carousel2.jpg">
          <div class="absolute-center second-caption q-mr-xl">
            <div class="text-h2 text-center">MAY SALE</div>
            <div class="text-h5 text-center text-primary">
              Up to 50% Discount
            </div>
          </div>
        </q-carousel-slide>
        <q-carousel-slide :name="3" img-src="~assets/carousel4.jpeg">
          <div class="absolute-bottom third-caption">
            <div class="text-h2 text-center">MAY SALE</div>
            <div class="text-h5 text-center text-primary">
              Up to 50% Discount
            </div>
          </div>
        </q-carousel-slide>
        <!-- <q-carousel-slide :name="4" img-src="~assets/carousel4.jpg">
          <div class="absolute-center fourth-caption">
            <div class="text-subtitle1 text-center">
              Our top-most priority is to make you look handsome and stylish
            </div>
            <div class="text-h3 text-center">
              WE KNOW THE HAIRCUT THAT SUITS YOU
            </div>
            <q-btn
              label="Book Appointment"
              color="secondary"
              rounded
              class="q-my-lg"
            />
          </div>
        </q-carousel-slide> -->
      </q-carousel>
    </div>

    <!-- List of Items -->

    <div class="row">
      <div class="col-xs-12 col-sm-6 col-md-3 ">
        <q-card class="my-card q-mx-md q-my-md" flat bordered >
          <img src="~assets/tecno.jpg" height="250" />

          <div class="text-h5 text-start q-mx-md ">Tecno Spark</div>
          <div class="text-subtitle1 text-start text-bold q-mx-md">
            GHC 1,000
          </div>

          <q-card-actions align="right">
            <q-btn flat round color="red" icon="favorite" />
            <q-btn flat round color="teal" icon="shopping_cart" />
            <!-- <q-btn flat round color="primary" icon="share" /> -->
          </q-card-actions>
        </q-card>
      </div>
      <div class="col-xs-12 col-sm-6 col-md-3">
        <q-card class="my-card q-mx-md q-my-md" flat bordered>
          <img src="~assets/samsung.jpg" height="250" />

          <div class="text-h5 text-start q-mx-md">Samsung A14</div>
          <div class="text-subtitle1 text-start text-bold q-mx-md">
            GHC 1,000
          </div>

          <q-card-actions align="right">
            <q-btn flat round color="red" icon="favorite" />
            <q-btn flat round color="teal" icon="shopping_cart" />
            <!-- <q-btn flat round color="primary" icon="share" /> -->
          </q-card-actions>
        </q-card>
      </div>
      <div class="col-xs-12 col-sm-6 col-md-3">
        <q-card class="my-card q-mx-md q-my-md" flat bordered>
          <img src="~assets/riceCooker.jpg" height="250" />

          <div class="text-h5 text-start q-mx-md">Rice Cooker</div>
          <div class="text-subtitle1 text-start text-bold q-mx-md">
            GHC 1,000
          </div>

          <q-card-actions align="right">
            <q-btn flat round color="red" icon="favorite" />
            <q-btn flat round color="teal" icon="shopping_cart" />
            <!-- <q-btn flat round color="primary" icon="share" /> -->
          </q-card-actions>
        </q-card>
      </div>
      <div class="col-xs-12 col-sm-6 col-md-3">
        <q-card class="my-card q-mx-md q-my-md" flat bordered>
          <img src="https://cdn.quasar.dev/img/mountains.jpg" />

          <div class="text-h5 text-start q-mx-md">Infinix Hot 10 Lite</div>
          <div class="text-subtitle1 text-start text-bold q-mx-md">
            GHC 1,000
          </div>

          <q-card-actions align="right">
            <q-btn flat round color="red" icon="favorite" />
            <q-btn flat round color="teal" icon="shopping_cart" />
            <!-- <q-btn flat round color="primary" icon="share" /> -->
          </q-card-actions>
        </q-card>
      </div>
      <div class="col-xs-12 col-sm-6 col-md-3">
        <q-card class="my-card q-mx-md q-my-md" flat bordered>
          <img src="https://cdn.quasar.dev/img/mountains.jpg" />

          <div class="text-h5 text-start q-mx-md">Infinix Hot 10 Lite</div>
          <div class="text-subtitle1 text-start text-bold q-mx-md">
            GHC 1,000
          </div>

          <q-card-actions align="right">
            <q-btn flat round color="red" icon="favorite" />
            <q-btn flat round color="teal" icon="shopping_cart" />
            <!-- <q-btn flat round color="primary" icon="share" /> -->
          </q-card-actions>
        </q-card>
      </div>
      <div class="col-xs-12 col-sm-6 col-md-3">
        <q-card class="my-card q-mx-md q-my-md" flat bordered>
          <img src="https://cdn.quasar.dev/img/mountains.jpg" />

          <div class="text-h5 text-start q-mx-md">Infinix Hot 10 Lite</div>
          <div class="text-subtitle1 text-start text-bold q-mx-md">
            GHC 1,000
          </div>

          <q-card-actions align="right">
            <q-btn flat round color="red" icon="favorite" />
            <q-btn flat round color="teal" icon="shopping_cart" />
            <!-- <q-btn flat round color="primary" icon="share" /> -->
          </q-card-actions>
        </q-card>
      </div>
      <div class="col-xs-12 col-sm-6 col-md-3">
        <q-card class="my-card q-mx-md q-my-md" flat bordered>
          <img src="https://cdn.quasar.dev/img/mountains.jpg" />

          <div class="text-h5 text-start q-mx-md">Infinix Hot 10 Lite</div>
          <div class="text-subtitle1 text-start text-bold q-mx-md">
            GHC 1,000
          </div>

          <q-card-actions align="right">
            <q-btn flat round color="red" icon="favorite" />
            <q-btn flat round color="teal" icon="shopping_cart" />
            <!-- <q-btn flat round color="primary" icon="share" /> -->
          </q-card-actions>
        </q-card>
      </div>
      <div class="col-xs-12 col-sm-6 col-md-3">
        <q-card class="my-card q-mx-md q-my-md" flat bordered>
          <img src="https://cdn.quasar.dev/img/mountains.jpg" />

          <div class="text-h5 text-start q-mx-md">Infinix Hot 10 Lite</div>
          <div class="text-subtitle1 text-start text-bold q-mx-md">
            GHC 1,000
          </div>

          <q-card-actions align="right">
            <q-btn flat round color="red" icon="favorite" />
            <q-btn flat round color="teal" icon="shopping_cart" />
            <!-- <q-btn flat round color="primary" icon="share" /> -->
          </q-card-actions>
        </q-card>
      </div>
    </div>
  </q-page>
</template>
<style scoped>
.myCarousel {
  height: 100vh;
  width: 98.7vw;
  overflow-x: hidden;
}

.first-caption,
.second-caption,
.third-caption,
.fourth-caption {
  display: flex;
  flex-flow: column nowrap;
  padding: 12px;
  color: white;
  width: 100%;
  height: inherit;
  background-color: rgba(0, 0, 0, 0.6);
  align-items: center;
  justify-content: center;
}
</style>
<script>
import { ref, defineComponent } from "vue";

export default defineComponent({
  name: "IndexPage",
  setup() {
    const slide = ref(1);
    const autoplay = ref(true);

    return {
      slide,
      autoplay,
    };
  },
});
</script>
