<template>
  <header>
    <a href="#">
      <app-logo />
    </a>
    <nav>
      <ul>
        <li v-for="link in navLinks" :key="link.text">
          <a :href="link.url">
            <span>{{ link.sign }}</span> {{ link.text }}
          </a>
        </li>
      </ul>
    </nav>
    <action-button />
  </header>
</template>

<script>
import AppLogo from "@/components/icons/AppLogo.vue";
import ActionButton from "@/components/Common/ActionButton.vue";

export default {
  name: "MainNav",
  components: {
    AppLogo,
    ActionButton,
  },
  data() {
    return {
      navLinks: [
        { sign: "[0]", text: "About", url: "#about" },
        { sign: "[1]", text: "Experience", url: "#experience" },
        { sign: "[2]", text: "Work", url: "#work" },
        { sign: "[3]", text: "Contact", url: "#contact" },
      ],
    };
  },
};
</script>
