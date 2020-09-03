<template>
  <div class="about">
    <h1>This is an codemirro test page</h1>
    <codemirror v-model="code" :options="cmOption"></codemirror>
  </div>
</template>
<script lang="ts">
import {Component, Vue} from "vue-property-decorator";
import HelloWorld from "../components/HelloWorld.vue";

@Component({
  components: {
    HelloWorld
  }
})
export default class CodemirrorTest extends Vue {
  code = 'hi';
  cmOption = {
    tabSize: 4,
    styleActiveLine: true,
    lineNumbers: true,
    mode: 'python',
    theme:'dracula'
  }
}
</script>