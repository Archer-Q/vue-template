<template>
  <div class="home">
    <el-icon color="#409EFC" class="no-inherit" @click="handleAdd">
      <Share />
    </el-icon>
    <img alt="Vue logo" src="../assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js + TypeScript App"/>
  </div>
</template>

<script lang="ts">
import { Options, Vue } from 'vue-class-component';
import HelloWorld from '@/components/HelloWorld.vue'; // @ is an alias to /src

@Options({
  components: {
    HelloWorld,
  },
})
export default class HomeView extends Vue {
  handleAdd() {
    console.log(11)
  }
}
</script>
