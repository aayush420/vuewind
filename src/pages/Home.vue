<template>
    <div>
        <HelloWorld msg="Hello Vue 3 + Vite" />
        <VAlert text="Hello from the alert" />
        <VButton v-text="'Hello123'" @click="alertThis('Clicked the Button')" />
        <VInput placeholder="Enter Something Here" class="mx-2" />
        <VSelect />
        <VButton v-text="'Show Modal'" @click="showModal = true" class="ml-2" />
        <br />
        <VCard />
        <div class="p-2 m-2 shadow inline-block">
            <VRadio name="radio1" />
            <VRadio name="radio1" />
            <VRadio name="radio1" />
            <VRadio name="radio1" />
        </div>
        <div class="p-2 m-2 shadow inline-block">
            <VCheck name="check1" />
            <VCheck name="check1" />
            <VCheck name="check1" />
            <VCheck name="check1" />
        </div>
        <VModal
            @submit="showModal = false"
            @close="showModal = false"
            v-if="showModal"
        />
    </div>
</template>

<script>
import HelloWorld from "../components/HelloWorld.vue";
import VAlert from "../components/Alert.vue";
import VButton from "../components/Button.vue";
import VCard from "../components/Card.vue";
import VCheck from "../components/Check.vue";
import VInput from "../components/Input.vue";
import VModal from "../components/Modal.vue";
import VRadio from "../components/Radio.vue";
import VSelect from "../components/Select.vue";
export default {
    components: {
        HelloWorld,
        VAlert,
        VButton,
        VCard,
        VCheck,
        VInput,
        VModal,
        VRadio,
        VSelect,
    },
    data() {
        return {
            showModal: false,
        };
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