<template>
  <div class="w-full">
    <label for="id">{{ label }}</label>
    <input
      :id="id"
      type="text"
      class="p-2 rounded-md text-neutral-900 w-full"
      :value="modelValue"
      @input="$emit('update:modelValue', $event.target.value)"
    />
  </div>
</template>

<script lang="ts">
export default {
  name: "AppTextInput",
  props: {
    label: { type: String, required: true },
    modelValue: { type: String, required: true },
  },
  emits: ["update:modelValue"],
  data() {
    return { id: 1 };
  },
};
</script>
