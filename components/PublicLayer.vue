<template>
  <div>
    <h1>Hello</h1>
    <p>
      This is called from Nuxt Public Layer:
      https://github.com/hardik-affilium/nuxt-public-layer
    </p>
    <v-container>
      <v-row>
        <v-col cols="12" class="text-center"> This is testing row. </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script setup>
import { useAuthStore } from "@/stores/auth/useAuthStore";
const authStore = useAuthStore();

const testauth1 = () => {
  authStore.testAuth();
};
</script>
