<template>
    <VSuperCenter
        class="absolute top-0 left-0 w-full h-full bg-gray-700 bg-opacity-50"
    >
        <VCard class="bg-white">
            <template v-slot:footer>
                <VButton @click="closeModal" class="mr-2" danger
                    >Cancel</VButton
                >
                <VButton @click="submitModal">Submit</VButton>
            </template>
        </VCard>
    </VSuperCenter>
</template>

<script>
import VButton from "./Button.vue";
import VCard from "./Card.vue";
import VSuperCenter from "./layouts/SuperCenter.vue";
export default {
    components: { VButton, VCard, VSuperCenter },
    methods: {
        closeModal() {
            this.$emit("close");
        },
        submitModal() {
            this.$emit("submit");
        },
    },
};
</script>

<style>
</style>