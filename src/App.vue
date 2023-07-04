<template>
  <h1>Hello</h1>
  <form-app>
    <div class="help">
      <p>This is some help text.</p>
    </div>
    <div class="fields">
      <input type="text" placeholder="email" />
      <input type="text" placeholder="username" />
      <input type="password" placeholder="password" />
    </div>
    <div class="buttons">
      <button type="button">submit</button>
    </div>
  </form-app>
  <form-app></form-app>
</template>

<script>
import FormApp from "@/components/Form.vue";

export default {
  name: "App",
  components: {
    FormApp,
  },
};
</script>
