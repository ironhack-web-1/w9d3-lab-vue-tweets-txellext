<template>
  <div className="tweet">
    <ProfileImage :image="user.image" />

    <div className="body">
      <div className="top">
        <User :userData="user" />

        <Timestamp :time="timestamp" />
      </div>

      <Message :message="message" />

      <div>
        <Actions />
      </div>
    </div>

    <i class="fas fa-ellipsis-h"></i>
  </div>
</template>

<script>
import ProfileImage from './ProfileImage.vue';
import User from './User.vue';
import Timestamp from './Timestamp.vue';
import Message from './Message.vue';
import Actions from './Actions.vue';

export default {
  props: ["user", "message", "timestamp"],
  components: {ProfileImage, User, Timestamp, Message, Actions}
}

</script>


<style scoped>
a {
  color: #42b983;
}
</style>
