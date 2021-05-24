<template>
  <router-view></router-view>
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";


@Options({
  components: {},
})
export default class App extends Vue {

}
</script>

<style lang="scss">
#app {
  font-family: Montserrat, Lato, Roboto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  background-color: #594f4f;
  background-image: linear-gradient(
    #e5fcc2,
    #9de0ad,
    #45ada8,
    #547980,
    #594f4f,
    #000f32
  );
}

@font-face {
  font-family: Montserrat;
  src: local("Montserrat"), url("./fonts/Montserrat-Regular.ttf");
}

#nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
