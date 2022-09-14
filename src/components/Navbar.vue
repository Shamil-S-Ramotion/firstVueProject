<template>
  <div class="navbar">
    <div @click="$router.push('/')">Inst</div>
    <div class="navbar__btns">
      <my-button @click="$router.push('/posts')">Posts</my-button>
      <my-button @click="$router.push('/about')" style="margin-left: 20px"
        >About</my-button
      >
    </div>
  </div>
</template>

<script>
import MyButton from "@/components/UI/MyButton";
export default {
  components: { MyButton },
};
</script>

<style scoped>
.navbar {
  height: 50px;
  background: gray;
  box-shadow: 2px 2px 4px gray;
  display: flex;
  align-items: center;
  padding: 0 15px;
}
.navbar__btns {
  margin-left: auto;
}
</style>
