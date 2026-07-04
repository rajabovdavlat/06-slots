<template>
  <div>
    <from-helper>
      <div slot="form-header">
        <h3>This is the title of the form</h3>
        <p>information about the formn</p>
      </div>
      <div slot="form-fields">
        <input type="text" placeholder="name" required />
        <input type="password" placeholder="password" required />
      </div>
      <div slot="form-controls">
        <button v-on:click="handleSubmit">Submit</button>
      </div>
    </from-helper>
  </div>
</template>

<script>
import fromHelper from "./components/fromHelper.vue";
export default {
  components: {
    "from-helper": fromHelper,
  },
  data() {
    return {};
  },
  methods: {},
};
</script>

<style></style>
