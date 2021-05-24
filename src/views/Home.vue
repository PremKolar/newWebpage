<template>
  <div>
    <div class="header"></div>
    <SlickCV :resume="resume"></SlickCV>
  </div>
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";
import HelloWorld from "@/components/HelloWorld.vue"; // @ is an alias to /src
import resumeData from "@/assets/resume.json";
import SlickCV from "@/components/slickCV/SlickCV.vue";

@Options({
  components: {
    HelloWorld,
    SlickCV,
  },
})
export default class Home extends Vue {
  private resume = resumeData;
}
</script>

<style type="text/css">
.header {
  /*background-image: url("../assets/goldenIndo_small.jpg");*/
  /*height: 486px;*/
  height: 3000px;
}
</style>
