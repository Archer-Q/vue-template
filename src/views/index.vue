<template>
  <div class="home">
    <el-icon color="#409EFC" class="no-inherit" @click="handleAdd">
      <Share />
    </el-icon>
    <PubAddForm msg="Welcome to Your Vue.js + TypeScript App"/>
  </div>
</template>

<script lang="ts">
import { Options, Vue } from 'vue-class-component';
import PubAddForm from '@/components/pubAddForm.vue'; // @ is an alias to /src

@Options({
  components: {
    PubAddForm,
  },
})
export default class HomeView extends Vue {
  handleAdd() {
    console.log(11)
  }
}
</script>
