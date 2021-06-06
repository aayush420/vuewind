<template>
    <button
        :class="`
            text-white
            bg-${color}-500
            border-0
            py-1
            px-6
            focus:outline-none
            hover:bg-${color}-600
            active:bg-${color}-700
            rounded
            shadow-lg`"
    >
        <slot></slot>
    </button>
</template>

<script>
export default {
    props: {
        primary: Boolean,
        success: Boolean,
        danger: Boolean,
    },
    computed: {
        color() {
            if (this.primary) return "indigo";
            else if (this.success) return "green";
            else if (this.danger) return "red";
            else return "indigo";
        },
    },
};
</script>

<style>
</style>