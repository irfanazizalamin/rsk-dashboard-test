<template>
  <div class="job-card">
    <img
      src="../../../assets/img/job-image.jpeg"
      class="job-card__img"
      alt="belum"
    />

    <div class="job-card__info">
      <h5 class="job-card__title">{{ title }}</h5>
      <div class="job-card__company">{{ company }}</div>
      <div class="job-card__posting">Diposting {{ posting }}</div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'JobCard',
  props: {
    title: {
      type: String,
      required: true,
    },
    company: {
      type: String,
      required: true,
    },
    posting: {
      type: String,
      required: true,
    },
  },
};
</script>

<style lang="scss">

@media only screen and (min-width: 768px) {
  .job-card:nth-child(odd) {
    padding: 20px 40px 20px 0;
  }

  .job-card:nth-child(even) {
    padding: 20px 40px 20px 20px;
  }
}

.job-card {
  display: flex;
  padding: 20px 0;

  &__img {
    background-color: green;
    width: 140px;
    border-radius: 16%;
  }

  &__info {
    margin-left: 40px;
    align-self: center;

    div {
      font-size: 18px;
      font-weight: 300;
      color: #707070;
    }

    .job-card__company {
      margin-bottom: 20px;
    }
  }
}
</style>
