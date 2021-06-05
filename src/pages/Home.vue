<template>
    <div>
        <HelloWorld msg="Hello Vue 3 + Vite" />
        <VAlert text="Hello from the alert" />
        <VButton v-text="'Hello123'" @click="alertThis('Clicked the Button')" />
        <VInput placeholder="Enter Something Here" class="mx-2" />
    </div>
</template>

<script>
import HelloWorld from "../components/HelloWorld.vue";
import VButton from "../components/Button.vue";
import VAlert from "../components/Alert.vue";
import VInput from "../components/Input.vue";
export default {
    components: {
        HelloWorld,
        VButton,
        VAlert,
        VInput
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