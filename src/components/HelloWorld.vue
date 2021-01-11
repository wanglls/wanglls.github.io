<template>
  <div class="hello">
    <!-- <h1>{{ msg }}</h1> -->
    <el-row type="flex" class="row-bg" justify="center">
      <el-col :span="12">
        <el-button type="primary" round>开始创作</el-button>
        <el-input
          type="textarea"
          :autosize="{ minRows: 2, maxRows: 4 }"
          placeholder="请输入内容"
          v-model="textarea2"
        >
        </el-input>
      </el-col>
    </el-row>
  </div>
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";

@Options({
  props: {
    msg: String,
  },
})
export default class HelloWorld extends Vue {
  msg!: string;
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
