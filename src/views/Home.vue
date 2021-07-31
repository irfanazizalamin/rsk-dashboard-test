<template>
  <div class="home">
    <navbar />

    <carousel />

    <div class="home__content">
      <class-category class="home__content-item" />

      <content-wrapper
        class="home__content-item"
        title="Kelas Terbaru"
        :content-data="newClassList"
      />

      <content-wrapper
        class="home__content-item"
        title="Bisnis dan Keuangan"
        :content-data="businessList"
      />

      <content-wrapper
        class="home__content-item"
        title="Kelas Terbaru"
        :content-data="marketingList"
      />
    </div>

    <job-vacancy class="home__job-vacancy" />

    <mitra class="home__mitra" />

    <Footer />

    <div class="home__help-button">
      <button type="button" class="btn">
        <img src="../assets/img/icons/bisnis.svg" alt="help" height="20">
        Help
      </button>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import Navbar from '../components/Navbar.vue';
import ClassCategory from '../components/class_category/ClassCategory.vue';
import ContentWrapper from '../components/content/ContentWrapper.vue';
import JobVacancy from '../components/job_vacancy/JobVacancy.vue';
import Mitra from '../components/mitra/Mitra..vue';
import Footer from '../components/Footer.vue';
import Carousel from '../components/carousel/Carousel.vue';

export default {
  name: 'Home',
  components: {
    Navbar,
    ClassCategory,
    ContentWrapper,
    JobVacancy,
    Mitra,
    Footer,
    Carousel,
  },
  data() {
    return {
      // kelas terbaru
      newClassList: [
        {
          title: 'Berdagang Hewan Kurban untuk Menjadi Pebisnis Ternak Hewan',
          price: 'Rp250.000',
        },
        {
          title: 'Menjadi Pedagang Cabai',
          price: 'Rp280.000',
        },
        {
          title: 'Menjadi Pedagang Hidroponik',
          price: 'Rp280.000',
        },
        {
          title: 'Menjadi Pengusaha Laptop',
          price: 'Rp210.000',
        },
        {
          title: 'Ternak Lele',
          price: 'Rp1.000',
        },
        {
          title: 'Menjadi Pedagang Cabai',
          price: 'Rp280.000',
        },
      ],
      // bisnis dan keuangan
      businessList: [
        {
          title: 'Bisnis Hewan Kurban',
          price: 'Rp250.000',
        },
        {
          title: 'Bisnis Ternak Lele',
          price: 'Rp280.000',
        },
        {
          title: 'Bisnis Mangga Muda',
          price: 'Rp280.000',
        },
        {
          title: 'Bisnis Manisan',
          price: 'Rp210.000',
        },
        {
          title: 'Bisnis Rujak',
          price: 'Rp1.000',
        },
        {
          title: 'Bisnis Selimut',
          price: 'Rp280.000',
        },
      ],
      // pemasaran
      marketingList: [
        {
          title: 'Menguasai Marketing',
          price: 'Rp250.000',
        },
        {
          title: 'Marketing dari 0',
          price: 'Rp280.000',
        },
        {
          title: 'Muda Berkarya',
          price: 'Rp280.000',
        },
        {
          title: 'Marketing sampai mati',
          price: 'Rp210.000',
        },
        {
          title: 'Marketing Internasional',
          price: 'Rp1.000',
        },
        {
          title: 'EZ Marketing',
          price: 'Rp280.000',
        },
      ],
    };
  },
};
</script>

<style lang="scss">
.home {
  &__content {
    padding: 40px 132px;

    &-item {
      margin-bottom: 40px;
    }
  }

  &__job-vacancy {
    padding: 40px 140px;
    background-color: rgba(128, 128, 128, 0.1);
  }

  &__mitra {
    padding: 40px 140px;
  }

  &__help-button {
    button {
      border-radius: 20px;
      background-color: #1F73B7 !important;
      color: #FFFFFF !important;
      fill: #FFFFFF !important;
      padding: 8px 20px;
      border-radius: 999rem;
    }
    position: fixed;
    bottom: 20px;
    right: 20px;
  }
}
</style>
