<template>
  <div>
    <the-header></the-header>
    <!-- or we can use it as - <TheHeader /> -->
    <badge-list></badge-list>
    <user-info
      :full-name="activeUser.name"
      :info-text="activeUser.description"
      :role="activeUser.role"
    ></user-info>
  </div>
</template>

<script>
import TheHeader from "./components/TheHeader.vue";
import BadgeList from "./components/BadgeList.vue";
import UserInfo from "./components/UserInfo.vue";

export default {
  components: {
    TheHeader,
    BadgeList,
    UserInfo,
  },
  data() {
    return {
      activeUser: {
        name: "Maximilian Schwarzmüller",
        description: "Site owner and admin",
        role: "admin",
      },
    };
  },
};
</script>

<!-- If we use <script scoped> </script>  then it will be treated as a local style for that particular component-->
<style>
html {
  font-family: sans-serif;
}

body {
  margin: 0;
}
</style>
