<template>
  <h1>This is user {{ $route.params.id }}</h1>
</template>
<script>
export default {
  validate(data) {
    console.log(data);
    return true;
  },
};
</script>
