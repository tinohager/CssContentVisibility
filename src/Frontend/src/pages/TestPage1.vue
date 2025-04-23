<template>
  <q-page>
    <div
      v-for="index in 10000"
      :key="index"
      class="box"
      :class="index % 2 === 0 ? 'box-green' : 'box-blue'"
    >
      box{{ index }}
      <div style="height: 100px">test</div>
    </div>
  </q-page>
</template>

<style scoped>
.box {
  content-visibility: auto;
  contain-intrinsic-size: auto 102px;
}

.box-green {
  background-color: aquamarine;
}

.box-blue {
  background-color: dodgerblue;
}
</style>
