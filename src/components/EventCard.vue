<template>
<div class="event-card card">
  <div class="card-header">{{event.categorie}}</div>
  <div class="card-body">
    <h5 class="card-title">{{event.title}}</h5>
    <p class="card-text">@ {{event.time}} on {{event.date}}.</p>
    <a href="#" class="btn btn-primary">add</a>
    <a href="#" class="btn btn-danger">delete</a>
    <a href="#" class="btn btn-warning">edit</a>
  </div>
</div>
  <!-- <div class="event-card">
    <span>@ {{event.time}} on {{event.date}}</span>
  <h4>{{event.title}}</h4>
  </div> -->
</template>

<script>
export default {
  name: "EventCard",
  props:{
    event:Object,
  }
 
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.event-card{
padding: 20px;
width:250px;
cursor: pointer;
border: 1px solid black;
margin-bottom: 18px;

}
.event-card:hover{
  transform: scale(1.01);
  box-shadow: 0 3px 12px 0 rgba(0, 0, 1, 0);
}
</style>
