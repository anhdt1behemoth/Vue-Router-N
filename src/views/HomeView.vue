<template>
  <div class="home">
    <h1>Home</h1>
   <button @click="$router.push('/user')">User</button>
  </div>
</template>

<script>
export default {
  name: 'HomeView',
  methods: {
    gotoUserPage() {
      this.$router.push({
        name: 'user',
        path: '/user',
        query: {id: 12341234}
      })
    }
  }
}
</script>
