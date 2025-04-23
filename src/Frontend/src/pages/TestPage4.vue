<template>
  <q-page>
    1000 Elements
    <div
      v-for="index in 1000"
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
}

.box-green {
  background-color: aquamarine;
}

.box-blue {
  background-color: dodgerblue;
}
</style>
