<template>
    <div
        class="
            absolute
            top-0
            left-0
            w-full
            h-full
            grid
            place-items-center
            bg-gray-700 bg-opacity-50
        "
    >
        <VCard class="bg-white">
            <template v-slot:footer>
                <VButton @click="closeModal" class="mr-2" danger
                    >Cancel</VButton
                >
                <VButton @click="submitModal">Click</VButton>
            </template>
        </VCard>
    </div>
</template>

<script>
import VButton from "./Button.vue";
import VCard from "./Card.vue";
export default {
    components: { VButton, VCard },
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