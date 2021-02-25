<template>
    <footer class="footer q-mt-xl">
        <div class="customContainer">
            <div class="row justify-center q-col-gutter-lg q-pa-lg">
                <div class="col-md-3">
                <h6 class="cardHeading q-pb-sm"> Information </h6>
                <q-list>
                    <q-item  clickable v-ripple v-for="info in information"  :key="info.item" class="q-pa-none">
                        <q-item-section class="linkItem q-py-xs">
                            {{info.item}}
                        </q-item-section>
                    </q-item>
                </q-list>
                </div>
                <div class="col-md-2">
                    <h6 class="cardHeading q-pb-sm"> Advertise with Us </h6>
                    <q-list>
                    <q-item  clickable v-ripple v-for="info in adcertise"  :key="info.item"  class="q-pa-none">
                        <q-item-section class="linkItem q-py-xs">
                            {{info.item}}
                        </q-item-section>
                    </q-item>
                </q-list>
                </div>
                <div class="col-md-2">
                <h6 class="cardHeading q-pb-sm"> Media </h6>
                <q-list>
                    <q-item  clickable v-ripple v-for="info in media"  :key="info.item"  class="q-pa-none">
                        <q-item-section class="linkItem q-py-xs">
                            {{info.item}}
                        </q-item-section>
                    </q-item>
                </q-list>
                </div>
                <div class="col-md-2">
                    <h6 class="cardHeading q-pb-sm">Venue Support </h6>
                    <q-list>
                    <q-item  clickable v-ripple v-for="info in support" :key="info.item"  class="q-pa-none">
                        <q-item-section class="linkItem q-py-xs">
                            {{info.item}}
                        </q-item-section>
                    </q-item>
                </q-list>
                </div>
                <div class="col-md-2">
                <h6 class="cardHeading q-pb-sm"> Company </h6>
                    <q-list>
                    <q-item  clickable v-ripple v-for="info in company" :key="info.item"  class="q-pa-none">
                        <q-item-section class="linkItem q-py-xs">
                            {{info.item}}
                        </q-item-section>
                    </q-item>
                </q-list>
                </div>
            </div>
           <q-separator inset></q-separator>
           <div class="q-pt-md row q-px-md">
               <div class="col-md-6">
                   <p>© 2021 VenueGPS</p>
                </div>
                <div class="col-md-6">
                    <div class="footerSocialShr float-right">
                        <q-icon class="q-px-xs" name="fab fa-facebook"></q-icon>
                        <q-icon class="q-px-xs" name="fab fa-twitter"></q-icon>
                        <q-icon class="q-px-xs" name="fab fa-instagram"></q-icon>
                        <q-icon class="q-px-xs" name="fab fa-youtube"></q-icon>
                        <q-icon class="q-px-xs" name="fab fa-snapchat"></q-icon>
                        <q-icon class="q-px-xs" name="fab fa-linkedin"></q-icon>
                    </div>
                </div>
           </div>

        </div>
    </footer>
</template>
<script>

export default {
  name: 'Footer',
  data: function () {
    return {
      information: [
        { item: 'Claim Business' },
        { item: 'Contact Us' },
        { item: "FAQ's" },
        { item: 'Privacy Policy' },
        { item: 'Terms of Use' }
      ],
      adcertise: [
        { item: 'Advertising Guidelines' },
        { item: 'Image Size Matrix' },
        { item: 'Our Logo' },
        { item: 'Pricing ' }
      ],
      media: [
        { item: 'Press Kit' },
        { item: 'Tutorial ' }
      ],
      support: [
        { item: 'SiteMap' },
        { item: 'Venue Live' },
        { item: 'Venue Aid' },
        { item: 'Venue Store' },
        { item: 'Venue Market' }
      ],
      company: [
        { item: 'CEO Message' },
        { item: 'Retired Digital' },
        { item: 'Career' },
        { item: 'About Us' },
        { item: 'Team' },
        { item: 'Vision' },
        { item: 'Sneak Preview' }
      ],
      slide: 1
    }
  }
}
</script>
