<template>
  <div class="home">
    <h1>Beer List</h1>
    <BeerList/>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';
import BeerList from '@/components/BeerList.vue';

export interface Beer {
  id: number;
  name: string;
  giphyUrl: string;
}

@Component({
  components: {
    BeerList,
  },
})

export default class Home extends Vue {
}
</script>
