<template>
  <div>
    <h1>Hello</h1>
    <pre>
This is called from Nuxt Public Layer: https://github.com/hardik-affilium/nuxt-public-layer</pre
    >
    <v-row>
      <v-col>
        <v-btn color="primary" @click="testauth1()">Test Button 2222</v-btn>
      </v-col>
    </v-row>
  </div>
</template>

<script setup>
import { useAuthStore } from "@/stores/auth/useAuthStore";
const authStore = useAuthStore();

const testauth1 = () => {
  authStore.testAuth();
};
</script>
