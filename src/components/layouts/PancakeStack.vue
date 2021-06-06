<template>
    <div class="pancake-stack parent">
        <slot name="header">
            <header
                class="bg-indigo-500 text-white h-24 grid place-items-center"
            >
                Header
            </header>
        </slot>
        <slot name="main">
            <main class="bg-coral-500 h-24 grid place-items-center">Main</main>
        </slot>
        <slot name="footer">
            <footer
                class="bg-purple-500 text-white h-24 grid place-items-center"
            >
                Footer Content
            </footer>
        </slot>
    </div>
</template>

<script>
// 04. Pancake Stack https://1linelayouts.glitch.me/
export default {};
</script>

<style>
.pancake-stack.parent {
    display: grid;
    grid-template-rows: auto 1fr auto;
}
</style>