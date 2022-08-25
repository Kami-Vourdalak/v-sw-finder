<template>
  <div class="flex items-end w-full">
    <app-text-input
      label="Search films by title, characters or planets."
      v-model="searchText"
    />
    <button class="p-2 bg-gray-700 rounded bg-yellow-200 text-neutral-900">
      Go
    </button>
  </div>
</template>

<script lang="ts">
import AppTextInput from "@/components/AppTextInput/AppTextInput.vue";
export default {
  name: "SearchFilms",
  components: { AppTextInput },
  data() {
    return { searchText: "" };
  },
};
</script>
