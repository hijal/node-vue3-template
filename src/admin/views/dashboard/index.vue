<template>
  <div class="dashboard-container">
    <div class="dashboard-text">name: {{ username }}</div>
    <div>
      update element-plus to 1.2.+, add svg icon, icon-font is abandoned
    </div>
    <i class="el-icon-add-location">abandoned</i>
    <div>
      <el-icon>
        <Edit />
      </el-icon>
    </div>
  </div>
</template>

<script setup>
import { Edit } from "@element-plus/icons";
import { computed } from "vue";
import { useStore } from "vuex";
let store = useStore();
const username = computed(() => {
  return store.state.user.username;
});
</script>

<style lang="scss" scoped>
.dashboard {
  &-container {
    //margin: 30px;
  }
  &-text {
    font-size: 30px;
    line-height: 46px;
  }
}
</style>
