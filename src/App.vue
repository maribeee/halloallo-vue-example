<template>
  <main>
    <Event :events="events"></Event>
  </main>
</template>

<script>
import Event from './components/Event.vue';

export default {
  name: 'App',
  components: {
    Event
  },
  data() {
    return {
      events: [
        {
          "title": "event title",
          "image": "http://placekitten.com/200/200",
          "location": "Guidet tur pa Kronborg slot - Afstand 6,6 km",
          "date": "15 October, 2021",
          "time": "14:00",
          "description": "Lorem ipsum dolor sit amet, consectetur adipisicing elit. Accusamus amet dignissimos dolorem ea eius harum incidunt laudantium, nesciunt nobis provident quis ratione repudiandae sed temporibus ut? In libero magnam nobis? At beatae deleniti eaque earum excepturi exercitationem explicabo illo incidunt inventore maxime minima necessitatibus, non numquam placeat quasi quod reiciendis repellat repudiandae sapiente sed soluta tempore vel velit vero, voluptatem? Et illum ipsum labore nobis non officiis tempora? "
        },
        {
          "title": "other event title",
          "image": "http://placekitten.com/202/202",
          "location": "Guidet tur pa Kronborg slot - Afstand 6,6 km",
          "date": "15 October, 2021",
          "time": "14:00",
          "description": "Lorem ipsum dolor sit amet, consectetur adipisicing elit. Accusamus amet dignissimos dolorem ea eius harum incidunt laudantium, nesciunt nobis provident quis ratione repudiandae sed temporibus ut? In libero magnam nobis? At beatae deleniti eaque earum excepturi exercitationem explicabo illo incidunt inventore maxime minima necessitatibus, non numquam placeat quasi quod reiciendis repellat repudiandae sapiente sed soluta tempore vel velit vero, voluptatem? Et illum ipsum labore nobis non officiis tempora? "
        },
        {
          "title": "third other event title",
          "image": "http://placekitten.com/204/202",
          "location": "Guidet tur pa Kronborg slot - Afstand 6,6 km",
          "date": "15 October, 2021",
          "time": "14:00",
          "description": "Lorem ipsum dolor sit amet, consectetur adipisicing elit. Accusamus amet dignissimos dolorem ea eius harum incidunt laudantium, nesciunt nobis provident quis ratione repudiandae sed temporibus ut? In libero magnam nobis? At beatae deleniti eaque earum excepturi exercitationem explicabo illo incidunt inventore maxime minima necessitatibus, non numquam placeat quasi quod reiciendis repellat repudiandae sapiente sed soluta tempore vel velit vero, voluptatem? Et illum ipsum labore nobis non officiis tempora? "
        },
        {
          "title": "fourth other event title",
          "image": "http://placekitten.com/207/202",
          "location": "Guidet tur pa Kronborg slot - Afstand 6,6 km",
          "date": "15 October, 2021",
          "time": "14:00",
          "description": "Lorem ipsum dolor sit amet, consectetur adipisicing elit. Accusamus amet dignissimos dolorem ea eius harum incidunt laudantium, nesciunt nobis provident quis ratione repudiandae sed temporibus ut? In libero magnam nobis? At beatae deleniti eaque earum excepturi exercitationem explicabo illo incidunt inventore maxime minima necessitatibus, non numquam placeat quasi quod reiciendis repellat repudiandae sapiente sed soluta tempore vel velit vero, voluptatem? Et illum ipsum labore nobis non officiis tempora? "
        },
      ]
    }
  },
}
</script>

<style>
@import './assets/base.css';

#app {
  max-width: 1280px;
  margin: 0 auto;
  padding: 2rem;

  font-weight: normal;
}

header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

a,
.green {
  text-decoration: none;
  color: hsla(160, 100%, 37%, 1);
  transition: 0.4s;
}

@media (hover: hover) {
  a:hover {
    background-color: hsla(160, 100%, 37%, 0.2);
  }
}

@media (min-width: 1024px) {
  body {
    display: flex;
    place-items: center;
  }

  #app {
    display: grid;
    grid-template-columns: 1fr;
    padding: 0 2rem;
  }


}
</style>
