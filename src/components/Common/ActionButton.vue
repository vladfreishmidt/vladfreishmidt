<template>
  <a href="/CV_Vladyslav_Freishmidt.pdf" target="_blank" @click="go">Resume</a>
</template>

<script>
export default {
  name: "ActionButton",
  methods: {
    go() {
      console.log("heah");
    },
  },
};
</script>

<style scoped>
a {
  background: none;
  color: #e3ff73;
  padding: 12px 18px;
  border: 1px solid #e3ff73;
  border-radius: 4px;
  cursor: pointer;
}

a:hover {
  background-color: rgba(227, 255, 115, 0.082);
}
</style>
