<template>
  <nav>
      <ul>
        <li v-for="route in routes">
          <router-link :to="route.path ? route.path : '/'">
            {{ route.titulo }}
          </router-link>
        </li>
      </ul>
    </nav>
</template>

<script>
export default {

  props: {
    routes: {
      type: Array,
      required: true
    }
  }
}
</script>

<style>

</style>
