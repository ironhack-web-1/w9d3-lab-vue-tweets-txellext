<template>
  <div className="tweet">
    <ProfileImage :image="user.image" />

    <div className="body">
      <div className="top">
        <User :userData="user" />

        <Timestamp :time="timestamp" />
      </div>

      <p className="message"> {{ message }} </p>

      <div className="actions">
        <!-- Font Awesome icons --> 
        <i class="far fa-comment"></i>
        <i class="fas fa-retweet"></i>
        <i class="far fa-heart"></i>
        <i class="fas fa-share"></i>
      </div>
    </div>

    <i class="fas fa-ellipsis-h"></i>
  </div>
</template>

<script>
import ProfileImage from './ProfileImage.vue';
import User from './User.vue';
import Timestamp from './Timestamp.vue';

export default {
  props: ["user", "message", "timestamp"],
  components: {ProfileImage, User, Timestamp}
}

</script>


<style scoped>
a {
  color: #42b983;
}
</style>
