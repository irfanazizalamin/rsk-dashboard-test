<template>
  <div class="content-wrapper">
    <div class="content-wrapper__header">
      <h3 class="content-wrapper__title">{{ title }}</h3>
      <div class="content-wrapper__see-all">Lihat Semua</div>
    </div>

    <div class="content-wrapper__content-wrapper-wrapper">
      <content-card
        class="content-wrapper__data"
        v-for="(data, i) in contentData"
        :data="data"
        :key="i"
      />
    </div>
  </div>
</template>

<script>
import ContentCard from './components/ContentCard.vue';

export default {
  name: 'ContentWrapper',
  props: {
    contentData: {
      type: Array,
      required: true,
    },
    title: {
      type: String,
      required: true,
    },
  },
  components: { ContentCard },
};
</script>

<style lang="scss">
.content-wrapper {
  &__title {
    margin-bottom: 20px;
  }

  &__header {
    display: flex;
    justify-content: space-between;
    align-items: center;

    .content-wrapper__see-all {
      color: blue;
      font-weight: 200;
      cursor: pointer;
    }
  }

  &__content-wrapper-wrapper {
    display: -webkit-box;
    overflow-x: scroll;
  }

  &__content-wrapper-wrapper::-webkit-scrollbar {
    display: none;
  }

  &__data {
    margin-right: 20px;
  }
}
</style>
