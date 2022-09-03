<template>
  <div>
    <img
      :src= "image"
      className="profile"
      alt="profile"
    />
  </div>
</template>

<script>
export default {
    props: ["image"]

}
</script>

<style>

</style>