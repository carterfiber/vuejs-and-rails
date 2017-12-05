<template>
  <div id="app" class="row">
    <div v-for="list in original_lists" class="col-md-4">
      
        <h2>{{ list.name}}</h2>
        <hr /> 
      <div class="well">
        <div v-for="(card, index) in list.cards">
        {{ card.name }}
        </div>
      </div> 
    </div>
  </div>
</template>

<script>
export default {
  props: ["original_lists"],
}
</script>

<style scoped>
p {
  font-size: 2em;
  text-align: center;
}
</style>
