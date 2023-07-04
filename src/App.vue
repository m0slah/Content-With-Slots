<template>
  <h1>Hello</h1>
  <form-app>
    <template v-slot:help>
      <p>{{ help }}</p>
    </template>
    <template v-slot:fields>
      <input type="text" placeholder="email" />
      <input type="text" placeholder="username" />
      <input type="password" placeholder="password" />
    </template>
    <template v-slot:buttons>
      <button type="button">submit</button>
    </template>
    <p>Dummy text</p>
  </form-app>
  <form-app>
    <template v-slot:help>
      <p>This is contact help text.</p>
    </template>
    <template v-slot:fields>
      <input type="text" placeholder="name" />
      <input type="text" placeholder="message" />
    </template>
    <template v-slot:buttons>
      <button type="button">submit</button>
    </template></form-app
  >
</template>

<script>
import FormApp from "@/components/Form.vue";

export default {
  name: "App",
  components: {
    FormApp,
  },
  data() {
    return {
      help: "This is some help text.",
    };
  },
};
</script>
