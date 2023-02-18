<template>
  <svg
    width="43"
    height="37"
    viewBox="0 0 43 37"
    fill="none"
    xmlns="http://www.w3.org/2000/svg"
  >
    <path
      d="M6 32.5L23.5 2.5L41 32.5H6Z"
      :stroke="fillColor"
      stroke-width="2"
    />
    <path d="M0.5 32L17 4" :stroke="fillColor" />
    <path
      d="M20.0615 20.3275V26.8345H27.3515V28.7245H20.0615V37H17.7395V18.4105H28.688L28.4045 20.3275H20.0615Z"
      :fill="fillColor"
    />
  </svg>
</template>

<script>
export default {
  name: "AppLogo",
  props: {
    fillColor: {
      type: String,
      default: "#E3FF73",
    },
  },
};
</script>
