<template>
    <div class="deconstructed-pancake flex flex-wrap justify-center">
        <slot>
            <div class="h-24 bg-green-500 grid place-items-center rounded-lg">
                1
            </div>
            <div class="h-24 bg-green-500 grid place-items-center rounded-lg">
                2
            </div>
            <div class="h-24 bg-green-500 grid place-items-center rounded-lg">
                3
            </div>
        </slot>
    </div>
</template>

<script>
export default {};
</script>

<style>
.deconstructed-pancake div {
    flex: 1 1 150px; /*  Stretching: */
    flex: 0 1 150px; /*  No stretching: */
    margin: 5px;
}
</style>