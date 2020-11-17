<template>
  <div>
    <h1>Users Slug Detail : {{ id }}</h1>
    <nuxt-link to="/users"> Back </nuxt-link>
  </div>
</template>

<script>
export default {
  data() {
    return {
      id: this.$route.params.slug,
    }
  },
  validate({ params }) {
    return params.slug === '1'
  },
}
</script>
