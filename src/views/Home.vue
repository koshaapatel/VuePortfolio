<template>
  <b-container>
    <b-row>
      <b-col lg="4" class="pb-2">
        <b-button size="sm">Small Button</b-button>
      </b-col>
      <b-col lg="4" class="pb-2">
        <b-button>Default Button</b-button>
      </b-col>
      <b-col lg="4" class="pb-2">
        <b-button size="lg">Large Button</b-button>
      </b-col>
    </b-row>
    <p>Hello, Bootstrap-Vue</p>
    <h1>jaja</h1>
    <b-btn
      variant="primary"
      @click="showAlert = true"
      v-b-tooltip.hover
      title="This button triggers the alert"
      >Click
    </b-btn>
    <b-alert v-bind:show="showAlert" variant="success">
      You clicked the button!
    </b-alert>
  </b-container>
</template>

<script>
export default {
  data: () => ({
    showAlert: false
  })
};
</script>
