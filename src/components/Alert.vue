<template>
  <div class="bg-indigo-500 text-white p-2 my-2">
      {{text}}
  </div>
</template>

<script>
export default {
    props: {
        text: {
            default: "Hello! Here is an alert"
        }
    }
}
</script>

<style>

</style>