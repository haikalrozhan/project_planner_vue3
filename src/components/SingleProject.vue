<template>
  <div class="projects">
      <div class="actions">
          <h3 @click="showDetails = !showDetails">{{project.title}}</h3>
      </div>
      <div class="details" v-if="showDetails">
          <p>{{project.details}}</p>
      </div>
  </div>
</template>

<script>
export default {
props: ['project'],
data(){
    return{
        showDetails : false
    }
}
}

</script>

<style>
.projects{
background: white;
margin: 20px auto;
padding: 10px 20px;
border-radius: 4px;
box-shadow: 1px 2px 3px rgba(0,0,0,0.05);
border-left: 4px solid #e90074
}
h3{
    cursor: pointer;
}
</style>