<template>
  <div>
    <input type="text" v-model="userId" />
    <button @click="handleLoadUser">Load User</button>
  </div>
</template>

<script>
export default {
  name: "IndexPage",
  data() {
    return {
      userId: "",
    };
  },
  methods: {
    handleLoadUser() {
      console.log(`clicked load user : ${this.userId}`);
      this.$router.push(`/user/${this.userId}`);
    },
  },
};
</script>
