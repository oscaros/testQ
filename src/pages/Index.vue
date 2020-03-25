<template>
  <q-page class="flex flex-center">
   <q-page class="bg-blue-1 window-height window-width row justify-center items-center">
    <div class="column">
      <div class="row">
        <q-card square bordered class="q-pa-lg shadow-1">
          <q-card-section>
            <q-form class="q-gutter-md">
              <q-input square filled clearable v-model="email" type="email" label="email" />
              <q-input square filled clearable v-model="pass" type="password" label="password"/>
            </q-form>
          </q-card-section>
          <q-card-actions class="q-px-md">
            <q-btn  @click="login" color="blue-9" size="lg" class="full-width" label="Login" />
          </q-card-actions>
          <q-card-section class="text-center q-pa-none">
            <div @click="register" class="text-grey-6">Not registered? Create an Account</div>
          </q-card-section>
        </q-card>
      </div>
    </div>
  </q-page>
  </q-page>
</template>
<script>
export default {
  name: 'PageIndex',
  data () {
    return {
      email: 'input your email',
      pass: 'pass'
    }
  },
  methods: {
    login () {
      console.log(this.email)
    },
    register () {
      console.log(this.pass)
    }
  }
}
</script>
