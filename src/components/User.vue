<template>
  <div>
    <span className="user">
          <span className="name"> {{ userData.name }}</span>
          <span className="handle">@{{ userData.handle }}</span>
        </span>
  </div>
</template>

<script>
export default {
    props: [ "userData" ]

}
</script>

<style>

</style>