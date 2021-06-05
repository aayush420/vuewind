<template>
  <div>
  <HelloWorld msg="Hello Vue 3 + Vite" />

  <VButton v-text="'Hello123'" @click="alertThis('Clicked the Button')" />

  </div>
</template>

<script>
import HelloWorld from '../components/HelloWorld.vue'
import VButton from '../components/Button.vue'
export default {
    components: {
        HelloWorld,
        VButton
    },
methods: {
    alertThis(msg) {
        alert(`Here is the msg - ${msg}`)
    }
}
}
</script>

<style>

</style>