<template>
  <div>
    <div>
        <a href="#" @click="fullHeight = true">Signin</a>
    </div>
    <q-dialog
      v-model="fullHeight"
      class="z-max"
    >
      <q-card class="column z-max " style="width: 800px;">
        <q-tab-panels v-model="tab" animated>
          <q-tab-panel name="signin">
           <Signin />
          </q-tab-panel>

          <q-tab-panel name="signup">
           <SignUp />
          </q-tab-panel>
        </q-tab-panels>
         <q-separator></q-separator>

        <q-tabs
          v-model="tab"
          dense
          class="bg-grey-3"
          align="justify"
          narrow-indicator
        >
          <q-tab name="signin" label="Sign In"></q-tab>
          <q-tab name="signup" label="Sign Up"></q-tab>
        </q-tabs>
        <q-card-actions align="right" class="bg-white text-teal">
          <q-btn flat label="close" v-close-popup></q-btn>
        </q-card-actions>
      </q-card>
    </q-dialog>
  </div>
</template>

<script>
import Signin from './signin'
import SignUp from './signup'
export default {
  name: 'auth',
  components: { Signin, SignUp },
  data () {
    return {
      fullHeight: false,
      tab: 'signin'
    }
  }
}
</script>
