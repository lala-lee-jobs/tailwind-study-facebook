<template>
  <div>
    <create-post class="card"></create-post>
    <live-chat class="card flex pr-0"></live-chat>
    <posts-wrapper></posts-wrapper>
  </div>
</template>

<script>
  import CreatePost from './create-post';
  import LiveChat from './live-chat';
  import PostsWrapper from './posts-wrapper';
  export default {
    name: 'PostsWall',
    components: { CreatePost, LiveChat, PostsWrapper },
  };
</script>

<style></style>
