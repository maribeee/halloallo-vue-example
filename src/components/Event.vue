<template>

  <div class="event" v-for="event in events">
    <div class="img">
      <img :src="event.image" alt=""/>
    </div>

    <div class="info">
      <div class="row title-row">
        <div class="col"><h3>{{ event.title }}</h3></div>
        <div class="col"><h3>{{ event.location }}</h3></div>
        <div class="col"><h3>{{ event.date }} at {{ event.time }}</h3></div>
      </div>

      <div class="row">
        <p>{{ event.description }}</p>
      </div>
    </div>
  </div>

</template>

<script>
export default {
  name: "Event",
  props: {
    events: JSON,
  }
}
</script>

<style lang="scss" scoped>
.event {
  display: flex;
  flex-direction: row;
  margin-bottom: 50px;

  .img {
    flex: 1;
  }

  .info {
    flex: 3;

    .row {
      display: flex;
      flex-direction: row;
      font-weight: 400;
      margin-bottom: 20px;
      justify-content: space-between;

      .title-row {
        font-weight: 700;
      }
    }

  }

}
</style>
