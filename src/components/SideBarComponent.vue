<template>
  <!-- sub-component within the body use vbase-css to autofill -->
  <div>
    <!-- things in html of this component -->
    <p>Side bar things</p>
    <p>Lots of things</p>
    <p>More side bar things</p>
  </div>
</template>

<script>
export default {
  //name of this component for use when exporting
  name: "side-bar-component",
};
</script>

<style scoped>
/* styling for THIS component only (only divs in 'SideBarComponent') */
div {
  display: grid;
  row-gap: 20px;
}
</style>
