<template>
  <div class="container event py-5"> 
    <h1>Liste des Evenements</h1>
    <EventCard v-for="event in events" :key="event.id" :event="event" />
  </div>
</template>

<script>
// @ is an alias to /src
import EventCard from "@/components/EventCard.vue";

export default {
  name: "EventList",
  components: {
    EventCard,
  },
  data() {
    return {
      // "events": [
      //   {
      //     "id": 0,
      //     "categorie": "bien-etre animal",
      //     "title": "journée dadoption des chats",
      //     "description": "trouvez votre nouvel ami felin lors de cet evenement",
      //     "location": "Bizerte",
      //     "date": "7 january 2022",
      //     "time": "12:00",
      //     "petsAllowed": true,
      //     "organizer": "foulen ben foulen",
      //   },
      //   {
      //     "id": 1,
      //     "categorie": "bien-etre animal",
      //     "title": "journée dadoption des chats",
      //     "description": "trouvez votre nouvel ami felin lors de cet evenement",
      //     "location": "Bizerte",
      //     "date": "28 january 2022",
      //     "time": "17:00",
      //     "petsAllowed": true,
      //     "organizer": "foulen ben foulen",
      //   },
      //   {
      //     "id": 2,
      //     "categorie": "bien-etre animal",
      //     "title": "anniversaire de balssem",
      //     "description": "trouvez votre nouvel ami felin lors de cet evenement",
      //     "location": "Bizerte",
      //     "date": "5 january 2022",
      //     "time": "16:00",
      //     "petsAllowed": true,
      //     "organizer": "foulen ben foulen",
      //   },
      // ],  
    };
  },
};
</script>
<style scoped>
.event{
  display: flex;
  flex-direction: column;
  align-items:center;
}
</style>
