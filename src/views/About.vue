<template>
  <div class="about">
    <h1>This is an about page</h1>
    <v-stage :config="stageStyle">
      <v-layer>
        <v-rect :config="rectStyle"></v-rect>
      </v-layer>
    </v-stage>
  </div>
</template>

<script>
export default {
  computed: {
    stageStyle() {
      return {
        width: 500,
        height: 300,
        draggable: true,
      };
    },
    rectStyle() {
      return {
        width: 20,
        height: 20,
        fill: 'red',
      };
    },
  },
};
</script>
