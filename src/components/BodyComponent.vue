<template>
  <!-- vbase-css to autofill -->
  <div>
    <!-- things in html of this component -->
    <br /><br />
    <p>This and the following are part of the the body</p>
    <div id="sectionContainer">
      <div>
        <div>
          <!-- using the team component in this place in the html of the body -->
          <team-component />
          <!-- using the fun component in this place in the html of the body -->
          <fun-component />
        </div>
      </div>
      <div id="pageRight">
        <!-- using the side bar component in this place in the html of the body -->
        <side-bar-component />
      </div>
    </div>
  </div>
</template>

<script>
//importing the sub components of this page
import FunComponent from "./FunComponent";
import TeamComponent from "./TeamComponent.vue";
import SideBarComponent from "./SideBarComponent.vue";
//register the new components in this page so we can use it in our HTML
export default {
  //register this component for use when exporting
  name: "body-component",
  components: {
    //resgister the components within this component
    TeamComponent,
    FunComponent,
    SideBarComponent,
  },
};
</script>
<style scoped>
/* styling for THIS component only */
#sectionContainer {
  display: grid;
  place-items: center;
  margin-top: 30px;
  grid-template-columns: 80% 1fr;
}
#pageRight {
  align-self: center;
  justify-self: end;
  width: 100%;
}
</style>
