<template>
  <div class="user">
      <h1>{{ user.email }}</h1>
  </div>
</template>

<script>
export default {
    name: 'user',
    props: {
        user: Object,
        default: null
    },
    data() {
        return {

        }
    }
}
</script>

<style>

</style>