<template>
    <h1>{{message}}</h1>
</template>

<script lang="ts">
  import { Vue } from 'nuxt-property-decorator';
  export default class extends Vue {
    private message: string = 'Hello!';
  }
</script>