<template>
  <div>
    <template v-for="(item, index) in list">
      <info-item v-bind="item" :key="`info-item-${index + 1}`"></info-item>
    </template>
  </div>
</template>

<script>
  import list from './list-data';
  import InfoItem from '@/components/common/info-item.vue';
  export default {
    name: 'LayoutMenuList',
    components: { InfoItem },
    data() {
      return {
        list,
      };
    },
  };
</script>

<style></style>
