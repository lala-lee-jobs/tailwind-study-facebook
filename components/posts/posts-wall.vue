<template>
  <div>
    <create-post class="card"></create-post>
    <create-chat class="card flex pr-0"></create-chat>
  </div>
</template>

<script>
  import CreatePost from './create-post';
  import CreateChat from './create-chat';
  export default {
    name: 'PostsWall',
    components: { CreatePost, CreateChat },
  };
</script>

<style></style>
