<template>
    <div>
        <HelloWorld msg="Hello Vue 3 + Vite" />
        <VAlert text="Hello from the alert" />
        <VButton v-text="'Hello123'" @click="alertThis('Clicked the Button')" />
        <VInput placeholder="Enter Something Here" class="mx-2" />
        <VSelect />
        <br />
        <VCard />
        <div class="p-2 m-2 shadow inline-block">
            <VRadio name="radio1" />
            <VRadio name="radio1" />
            <VRadio name="radio1" />
            <VRadio name="radio1" />
        </div>
    </div>
</template>

<script>
import HelloWorld from "../components/HelloWorld.vue";
import VAlert from "../components/Alert.vue";
import VButton from "../components/Button.vue";
import VInput from "../components/Input.vue";
import VSelect from "../components/Select.vue";
import VCard from "../components/Card.vue";
import VRadio from "../components/Radio.vue";
export default {
    components: {
        HelloWorld,
        VAlert,
        VButton,
        VInput,
        VSelect,
        VCard,
        VRadio,
    },
    methods: {
        alertThis(msg) {
            console.log(`Here is the msg - ${msg}`);
        },
    },
};
</script>

<style>
</style>