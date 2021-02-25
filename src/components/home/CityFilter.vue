<template>
<div class="citiesFilterWrap customContainer q-mb-md q-mt-md">
     <div class="citiesFilterHeading">
         <h4 class="q-mb-sm q-mt-lg headingH2"> Top Cities </h4>
     </div>
       <q-carousel
            v-model="slide"
            transition-prev="slide-right"
            transition-next="slide-left"
            swipeable
            animated
            control-color="white"
            control-type="square"
            control-text-color="grey-8"
            padding
            arrows
            height="auto"
            class=""
        >
        <q-carousel-slide :name="1" class="column no-wrap q-pl-none">
            <div class="row fit justify-start items-center q-gutter-md q-col-gutter no-wrap">
                <div class="col-md-3 col-sm-6 col-xs-12  full-height">
                    <q-img class="rounded-borders full-height" src="https://cdn.quasar.dev/img/mountains.jpg"></q-img>
                    <div>
                        <div class="cFcityName q-pt-sm cardHeading">
                            Austin
                        </div>
                        <div class="cFeventCount paragraphText">
                            43 Events
                        </div>
                    </div>
                </div>
                <div class="col-md-3 col-sm-6 col-xs-12  full-height">
                    <q-img class="rounded-borders full-height" src="https://cdn.quasar.dev/img/parallax1.jpg"></q-img>
                    <div>
                        <div class="cFcityName q-pt-sm cardHeading">
                            Austin
                        </div>
                        <div class="cFeventCount paragraphText">
                            43 Events
                        </div>
                    </div>
                 </div>
                <div class="col-md-3 col-sm-6 col-xs-12  full-height">
                    <q-img class="rounded-borders full-height" src="https://cdn.quasar.dev/img/mountains.jpg"></q-img>
                    <div>
                        <div class="cFcityName q-pt-sm cardHeading">
                            Austin
                        </div>
                        <div class="cFeventCount paragraphText">
                            43 Events
                        </div>
                    </div>
                </div>
                <div class="col-md-3 col-sm-6 col-xs-12  full-height">
                     <q-img class="rounded-borders full-height" src="https://cdn.quasar.dev/img/parallax1.jpg"></q-img>
                     <div>
                        <div class="cFcityName q-pt-sm cardHeading">
                            Austin
                        </div>
                        <div class="cFeventCount paragraphText">
                            43 Events
                        </div>
                    </div>
                </div>
            </div>
        </q-carousel-slide>

        <q-carousel-slide :name="2" class="column no-wrap q-pl-none">
            <div class="row fit justify-start items-center q-gutter-md q-col-gutter no-wrap">
                <div class="col-md-3 col-sm-6 col-xs-12  full-height">
                    <q-img class="rounded-borders full-height" src="https://cdn.quasar.dev/img/mountains.jpg"></q-img>
                    <div>
                        <div class="cFcityName q-pt-sm cardHeading">
                            Austin
                        </div>
                        <div class="cFeventCount paragraphText">
                            43 Events
                        </div>
                    </div>
                </div>
                <div class="col-md-3 col-sm-6 col-xs-12  full-height">
                    <q-img class="rounded-borders full-height" src="https://cdn.quasar.dev/img/parallax1.jpg"></q-img>
                    <div>
                        <div class="cFcityName q-pt-sm cardHeading">
                            Austin
                        </div>
                        <div class="cFeventCount paragraphText">
                            43 Events
                        </div>
                    </div>
                 </div>
                <div class="col-md-3 col-sm-6 col-xs-12  full-height">
                    <q-img class="rounded-borders full-height" src="https://cdn.quasar.dev/img/mountains.jpg"></q-img>
                    <div>
                        <div class="cFcityName q-pt-sm cardHeading">
                            Austin
                        </div>
                        <div class="cFeventCount paragraphText">
                            43 Events
                        </div>
                    </div>
                </div>
                <div class="col-md-3 col-sm-6 col-xs-12  full-height">
                     <q-img class="rounded-borders full-height" src="https://cdn.quasar.dev/img/parallax1.jpg"></q-img>
                     <div>
                        <div class="cFcityName q-pt-sm cardHeading">
                            Austin
                        </div>
                        <div class="cFeventCount paragraphText">
                            43 Events
                        </div>
                    </div>
                </div>
            </div>
        </q-carousel-slide>

        <q-carousel-slide :name="3" class="column no-wrap q-pl-none">
            <div class="row fit justify-start items-center q-gutter-md q-col-gutter no-wrap">
                <div class="col-md-3 col-sm-6 col-xs-12  full-height">
                    <q-img class="rounded-borders full-height" src="https://cdn.quasar.dev/img/mountains.jpg"></q-img>
                    <div>
                        <div class="cFcityName q-pt-sm cardHeading">
                            Austin
                        </div>
                        <div class="cFeventCount paragraphText">
                            43 Events
                        </div>
                    </div>
                </div>
                <div class="col-md-3 col-sm-6 col-xs-12  full-height">
                    <q-img class="rounded-borders full-height" src="https://cdn.quasar.dev/img/parallax1.jpg"></q-img>
                    <div>
                        <div class="cFcityName q-pt-sm cardHeading">
                            Austin
                        </div>
                        <div class="cFeventCount paragraphText">
                            43 Events
                        </div>
                    </div>
                 </div>
                <div class="col-md-3 col-sm-6 col-xs-12  full-height">
                    <q-img class="rounded-borders full-height" src="https://cdn.quasar.dev/img/mountains.jpg"></q-img>
                    <div>
                        <div class="cFcityName q-pt-sm cardHeading">
                            Austin
                        </div>
                        <div class="cFeventCount paragraphText">
                            43 Events
                        </div>
                    </div>
                </div>
                <div class="col-md-3 col-sm-6 col-xs-12  full-height">
                     <q-img class="rounded-borders full-height" src="https://cdn.quasar.dev/img/parallax1.jpg"></q-img>
                     <div>
                        <div class="cFcityName q-pt-sm cardHeading">
                            Austin
                        </div>
                        <div class="cFeventCount paragraphText">
                            43 Events
                        </div>
                    </div>
                </div>
            </div>
        </q-carousel-slide>
        </q-carousel>
     </div>
</template>
<script>
export default {
  name: 'CityFilter',
  data: function () {
    return {
      slide: 1
    }
  }

}
</script>
