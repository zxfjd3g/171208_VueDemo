<template>
  <ul>
    <li v-for="m in messages" :key="m.id">
      <router-link to="???">{{m.title}}</router-link>
    </li>
  </ul>
</template>

<script>
  export default {
    data () {
      return {
        messages: [
         /* {id: 1, title: 'Message001'},
          {id: 3, title: 'Message003'},
          {id: 5, title: 'Message005'}*/
        ]
      }
    },

    mounted () {
      setTimeout(() => {
        const messages = [
          {id: 1, title: 'Message001'},
           {id: 3, title: 'Message003'},
           {id: 5, title: 'Message005'}
        ]
        this.messages = messages
      }, 1000)
    }
  }
</script>

<style>

</style>