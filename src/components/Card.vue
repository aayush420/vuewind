<template>
    <div class="shadow inline-block p-2 m-2">
        <div class="text-xl">Card Title</div>
        <div class="">
            Card description goes here ..<br />One more line goes here ..
        </div>
        <footer>
            <slot name="footer"></slot>
        </footer>
    </div>
</template>

<script>
export default {};
</script>

<style>
</style>