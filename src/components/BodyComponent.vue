<template>
  <div>
    <p>This and the following are part of the the body</p>
    <!-- <div>
      <h2>Meet the team:</h2>
      <img
        alt="Josh the Doodle"
        src="https://www.storytrender.com/wp-content/uploads/2019/08/CATERS_DISABLED_GOLDEN_DOODLE_03.jpg"
      />
    </div> -->
    <!-- <div>
      <h2>
        Fun
      </h2>
      <img
        src="https://skatehut.images.blucommerce.com/skatehut/Blog/Arbor_LongB_1704_1.jpg?auto=format%2Ccompress&w=750&h=620&fit=fillmax&fill=solid&s=83970302f5da0cdb6420ccfaef9fc0fe"
        alt="longboards in a row"
      />
    </div> -->
    <div id="sectionContainer">
      <div>
        <div>
          <team-component />
          <fun-component />
        </div>
      </div>
      <div id="pageRight">
        <side-bar-component />
      </div>
    </div>
  </div>
</template>

<script>
import FunComponent from "./FunComponent";
import TeamComponent from "./TeamComponent.vue";
import SideBarComponent from "./SideBarComponent.vue";
export default {
  name: "body-component",
  components: {
    TeamComponent,
    FunComponent,
    SideBarComponent,
  },
};
</script>
<style scoped>
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
