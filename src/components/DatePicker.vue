<template>
    <div>
        <!-- <v-date-picker v-model="range" is-range /> -->
        <vc-calendar />
      <!-- <v-date-picker v-model="date" :mode="mode" is-inline /> -->
    </div>
</template>

<script>
export default {
  name: "DatePicker",
  data() {
    return {
      date: null,
      mode: "datetime",
    };
  },
};
</script>

<style scoped>
</style>