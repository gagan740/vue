<template>
  <div>
    <app-header v-bind:title="title"></app-header>
    <app-ninjas v-bind:ninjas="ninjas"></app-ninjas>
    <app-footer v-bind:title="title"></app-footer>
  </div>
</template>

<script>
import Header from './components/Header.vue';
import Footer from './components/Footer.vue';
import Ninjas from './components/Ninjas.vue';

export default {
  components: {
    'app-header': Header,
    'app-footer': Footer,
    'app-ninjas': Ninjas
  },
  data () {
    return {
      ninjas: [
          {name: 'Ryu', spaciality: 'Vue Components', show: false},
          {name: 'Crystal', spaciality: 'HTML Wizardry', show: false},
          {name: 'Hitoshi', spaciality: 'Click Events', show: false},
          {name: 'Tango', spaciality: 'Conditionals', show: false},
          {name: 'Kami', spaciality: 'Webpack', show: false},
          {name: 'Yoshi', spaciality: 'Data Diggin', show: false},
      ],
      title: "Vue Ninjas",
    }
  }
}
</script>

<style>

</style>
