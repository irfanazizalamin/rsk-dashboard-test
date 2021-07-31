<template>
  <div class="job-vacancy">
    <h3 class="job-vacancy__title">Lowongan Kerja</h3>

    <div class="job-vacancy__wrapper">
      <job-card
        class="job-vacancy__data"
        v-for="(job, i) in jobs"
        :key="i"
        :company="job.company"
        :title="job.title"
        :posting="job.posting"
      />
    </div>
  </div>
</template>

<script>
import JobCard from './components/JobCard.vue';

export default {
  name: 'JobVacancy',
  data() {
    return {
      jobs: [
        {
          title: 'Quality Assurance',
          company: 'PT Alba Integrasi Solusi',
          posting: '1 minggu yang lalu',
        },
        {
          title: 'Front End Developer',
          company: 'PT Alba Integrasi Solusi',
          posting: '1 minggu yang lalu',
        },
        {
          title: 'Android Developer',
          company: 'PT Alba Integrasi Solusi',
          posting: '1 minggu yang lalu',
        },
      ],
    };
  },
  components: {
    JobCard,
  },
};
</script>

<style lang="scss">
.job-vacancy {
  &__wrapper {
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    justify-content: left;
    margin: 0 15px;
  }
}
</style>
