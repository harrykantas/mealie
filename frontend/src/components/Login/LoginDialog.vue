<template>
  <div class="text-center">
    <v-dialog v-model="dialog" width="500px">
      <LoginForm @logged-in="dialog = false" />
    </v-dialog>
  </div>
</template>

<script>
import LoginForm from "./LoginForm";
export default {
  components: {
    LoginForm,
  },
  data() {
    return {
      dialog: false,
    };
  },
  methods: {
    open() {
      this.dialog = true;
    },
  },
};
</script>

<style></style>
