<template>
  <div>
    <h1>Users Index</h1>
    <ul>
      <li v-for="user in users" :key="user.id">
        <nuxt-link :to="`/users/${user.id}`">{{ user.id }}</nuxt-link>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      users: [{ id: 1 }, { id: 2 }, { id: 3 }],
    }
  },
}
</script>
