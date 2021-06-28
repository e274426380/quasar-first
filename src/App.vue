<template>
  <q-layout view="lHr lpR fFf">

    <q-header elevated class="bg-primary text-white">
      <q-toolbar>
        <q-toolbar-title>
          <q-avatar>
            <img src="https://cdn.quasar.dev/logo/svg/quasar-logo.svg">
          </q-avatar>
          Title
        </q-toolbar-title>
      </q-toolbar>
    </q-header>

    <q-drawer show-if-above v-model="left" side="left" behavior="desktop">
      <!-- drawer content -->
      <q-toolbar class="bg-primary text-white">
      </q-toolbar>
    </q-drawer>

    <q-drawer show-if-above v-model="right" side="right" behavior="desktop">
      <!-- drawer content -->
      <q-toolbar class="bg-primary text-white">
      </q-toolbar>
    </q-drawer>

    <q-page-container>
    </q-page-container>

  </q-layout>
</template>

<script>
  export default {
    data () {
      return {
        left: false,
        right: false
      }
    }
  }
</script>
