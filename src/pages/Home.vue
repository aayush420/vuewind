<template>
    <div>
        <HelloWorld msg="Hello Vue 3 + Vite" />
        <VAlert text="Hello from the alert" />
        <VButton v-text="'Hello123'" @click="alertThis('Clicked the Button')" />
    </div>
</template>

<script>
import HelloWorld from "../components/HelloWorld.vue";
import VButton from "../components/Button.vue";
import VAlert from "../components/Alert.vue";
export default {
    components: {
        HelloWorld,
        VButton,
        VAlert,
    },
    methods: {
        alertThis(msg) {
            alert(`Here is the msg - ${msg}`);
        },
    },
};
</script>

<style>
</style>