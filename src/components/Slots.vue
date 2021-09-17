<template>
  <section>
    <div :key="task.id" v-for="task in tasks">
      <img :src=task.img alt="">
      <h3>{{task.name}}</h3>
      <p>{{task.desc}}</p>
    </div>
  </section>
</template>

<script>
export default {
  name: 'Slots',
  props: {
    tasks: Array
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

  section{
    display: flex;
    justify-content: space-between;
  }

  div{
    width: 300px;
    margin: 1rem;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }

  img{
    height: 150px;
  }

</style>
