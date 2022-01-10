<template>
  <section>
    <vue-masonry-wall :items="items" :options="options" @append="append">
      <template v-slot:default="{item}">
        <div class="Item">
          <img :src="item.image"/>
        </div>
      </template>
    </vue-masonry-wall>
  </section>
</template>

<script>
import VueMasonryWall from "vue-masonry-wall";

export default {
  name: "ExampleMasonry",
  components: {VueMasonryWall},
  data() {
    return {
      options: {
        width: 300,
        padding: {
          2: 8,
          default: 12
        },
      },
      items: [
        {
          image: 'https://picsum.photos/id/1015/600/600'
        },
        {
          image: 'https://picsum.photos/id/1019/600/700'
        },
        {
          image: 'https://picsum.photos/id/1039/600/800'
        },
        {
          image: 'https://picsum.photos/id/1042/600/300'
        },
      ]
    }
  },
  methods: {
    append() {
      for (let i = 0; i < 20; i++) {
        const id = Math.floor(Math.random() * 1000)
        const height = Math.floor(Math.random() * 200) + 600
        this.items.push({
          image: `https://picsum.photos/id/${id}/600/${height}`
        })
      }
    }
  }
}
</script>

<style scoped>

.Item {
  overflow: hidden;
  border-radius: 4px;
  width: 100%;
  background: #F5F5F5;
}

img {
  object-fit: cover;
  width: 100%;
  height: 100%;
  line-height: 0;
  display: block;
}
</style>