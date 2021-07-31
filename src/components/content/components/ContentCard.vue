<template>
  <div class="content-card card" style="width: 16rem">
    <div class="content-card__thumb">
      <img
        src="../../../assets/img/sample-image.jpeg"
        class="content-card__thumb-img card-img-top"
        alt="sample-image"
      />

      <span class="content-card__thumb-type">Kelas Video</span>
    </div>

    <div class="content-card__body card-body">
      <div class="card-title">
        {{ data.title }}
      </div>

      <div class="content-card__price-container flex">
        <div class="price">
          <div class="card-price">{{ data.price }}</div>
        </div>
        <div class="rating">
          <div class="card-rating">
            <img
              src="../../../assets/img/icons/training-star.svg"
              alt="star-icon"
            />
            NEW
          </div>
        </div>
      </div>

      <div class="content-card__class-type">
        Kelas Video
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'ContentCard',
  props: {
    data: {
      type: Object,
      required: true,
    },
  },
};
</script>

<style lang="scss">
.card-title {
  font-size: 16px;
  line-height: 24px;
  margin-right: 4px;
  display: -webkit-box;
  -webkit-line-clamp: 2;
  -webkit-box-orient: vertical;
  overflow: hidden;
}

.flex {
  display: flex;
  justify-content: space-between;
}

.content-card {
  &__class-type {
    font-size: 18px;
    margin-bottom: 12px;
    color: #939393;
  }

  &__price-container {
    margin: 12px 0;
  }
}

.content-card__thumb {
  &-type {
    position: absolute;
    color: white;
    top: 6px;
    right: 6px;
    margin: 0;
    background: rgba(0, 0, 0, 0.5);
    padding: 4px 12px;
    border-radius: 4px;
    font-size: 12px;
    font-weight: 500;
  }

  &-info {
    position: absolute;
    display: flex;
    bottom: 0px;
    left: 6px;
    background-color: aqua;
  }

  &-img {
    background-color: aqua;
  }
}
</style>
