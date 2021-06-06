<template>
    <div class="sidebar-says parent">
        <slot name="sidebar">
            <div class="bg-yellow-400 p-4">Min: 150px / Max: 25%</div>
        </slot>
        <slot name="content">
            <div class="bg-purple-500 p-4 text-white">
                This element takes the second grid position (1fr), meaning it
                takes up the rest of the remaining space.
            </div>
        </slot>
    </div>
</template>

<script>
// 03. Sidebar Says https://1linelayouts.glitch.me/
export default {};
</script>

<style>
.sidebar-says.parent {
    display: grid;
    grid-template-columns: minmax(150px, 25%) 1fr;
}
</style>