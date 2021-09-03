<template>
  <div>
    <label :for="select">What {{ select }} do you want?</label>

    <select
      @change="$emit('change', $event.target.value)"
      :name="select"
      :id="select"
    >
      <option value>Please Select {{ select }}</option>
      <option v-for="option in selectOptions" :key="option" :value="option">
        {{ option }}
      </option>
    </select>
  </div>
</template>

<script>
export default {
  props: {
    select: {
      type: String,
      default: "cuison"
    },
    selectOptions: {
      type: Array,
      default: () => ["taco", "pizza", "dim sum"]
    }
  }
};
</script>

<style></style>
