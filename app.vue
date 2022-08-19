<script lang="ts" setup>
const textRef = ref(`# はじめに\n\n- これは箇条書き\n- 2つ目の箇条書き\n`);
</script>

<template>
  <div style="width: 640px; height: 480px; border: 1px solid">
    <ClientOnly>
      <LazyAppMonacoEditor
        language="markdown"
        v-model="textRef"
      ></LazyAppMonacoEditor>
    </ClientOnly>
  </div>
</template>
