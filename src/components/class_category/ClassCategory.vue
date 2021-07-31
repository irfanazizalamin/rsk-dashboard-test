<template>
  <div>
    <h3 class="class-category__title">Kategori Kelas</h3>
    <div class="class-category__list">
      <div
        v-for="(category, i) in classCategories" :key="i"
        class="class-category__list-data card"
      >
        <div class="card-horizontal">
          <div class="class-category__list-data__img">
            <img src="../../assets/img/icons/bahasa-asing.svg" alt="bahasa-asing" height="16">
          </div>

          <span class="class-category__list-data__text">{{ category.text }}</span>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'ClassCategory',
  data() {
    return {
      classCategories: [
        {
          text: 'Bahasa Asing',
          img: 'bahasa-asing',
        },
        {
          text: 'Bisnis & Keuangan',
          img: 'bisnins',
        },
        {
          text: 'Industri Kreatif',
          img: 'kreatif',
        },
        {
          text: 'Kesehatan & Kecantikan',
          img: 'kesehatan-kecantikan',
        },
        {
          text: 'Pariwisata & Pelayanan',
          img: 'ritel-layana',
        },
        {
          text: 'Pemasaran',
          img: 'pemasaran',
        },
        {
          text: 'Bahasa Asing',
          img: 'bahasa-asing',
        },
        {
          text: 'Bisnis & Keuangan',
          img: 'bisnins',
        },
      ],
    };
  },
};
</script>

<style lang="scss">
.card-horizontal {
  display: flex;
  flex: 1 1 auto;
}

.class-category {
  &__title {
    margin-bottom: 20px;
  }

  &__list {
    display: -webkit-box;
    overflow-x: hidden;
  }

  &__list:hover {
    overflow-x: scroll;
  }

  &__list-data {
    margin-right: 12px;
    padding: 8px 12px;
    background-color: #fff;
    border-radius: 5px;
    align-self: center;

    &__text {
      align-self: center;
      font-size: 12px;
      margin-left: 16px;
    }

    &__img {
      align-self: center;
    }
  }
}

.class-category__list::-webkit-scrollbar {
  height: 12px;
}

.class-category__list::-webkit-scrollbar-track {
  box-shadow: inset 0 0 10px 10px rgba(128, 128, 128, 0.4);
  border-radius: 12px;
  border: solid 3px transparent;
}

.class-category__list::-webkit-scrollbar-thumb {
  box-shadow: inset 0 0 10px 10px rgba(0, 0, 0, 0.4);
  border-radius: 12px;
  border: solid 3px transparent;
}
</style>
