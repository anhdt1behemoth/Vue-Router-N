<template>
  <div class="home">
    <h1>User {{$route.params.id}}</h1>
    <button @click="back">back</button>
  </div>
</template>

<script>
export default {
  props: ['id'],
  name: 'UserView',
  methods: {
    back() {
     alert(this.id)
    }
  }
}
</script>
