<template>
  <div>
    <create-post class="card"></create-post>
    <live-chat class="card flex pr-0"></live-chat>
  </div>
</template>

<script>
  import CreatePost from './create-post';
  import LiveChat from './live-chat';
  export default {
    name: 'PostsWall',
    components: { CreatePost, LiveChat },
  };
</script>

<style></style>
