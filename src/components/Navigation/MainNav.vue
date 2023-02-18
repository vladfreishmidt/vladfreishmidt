<template>
  <header class="container mx-auto flex h-20 items-center px-4">
    <a class="flex-grow" href="#">
      <app-logo />
    </a>
    <nav class="mr-8">
      <ul class="flex">
        <li v-for="link in navLinks" :key="link.text" class="ml-8 first:ml-0">
          <a :href="link.url" class="font-mono text-sm">
            <span>{{ link.sign }}</span>
            <span>{{ link.text }}</span>
          </a>
        </li>
      </ul>
    </nav>
    <action-button />
  </header>
</template>

<script>
import AppLogo from "@/components/Icons/AppLogo.vue";
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
