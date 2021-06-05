<template>
    <label
        class="
            ml-2
            text-sm
            font-medium
            text-gray-700
            flex
            items-center
            cursor-pointer
        "
    >
        <input
            type="checkbox"
            class="
                mr-2
                focus:ring-indigo-500
                h-4
                w-4
                text-indigo-600
                border-gray-300
            "
            :name="name"
        />
        Some radio option
    </label>
</template>

<script>
export default {
    props: ["name"],
};
</script>

<style>
</style>