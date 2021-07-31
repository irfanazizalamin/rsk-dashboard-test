<template>
  <div class="mitra">
    <h3 class="mitra__title">Mitra RSK</h3>
    <p>Rumah Siap Kerja dipercaya oleh institusi terbaik di Indonesia.</p>

    <div class="mitra__data">
      <div class="container">
        <div class="companies__outer">
          <div class="companies__outer--box">
            <img src="../../assets/img/ipb-logo.png" alt="ipb-logo">
          </div>
          <div class="companies__outer--box">
            <img src="../../assets/img/ui-logo.png" alt="ui-logo">
          </div>
          <div class="companies__outer--box">
            <img src="../../assets/img/tiktok-logo.png" alt="tiktok-logo">
          </div>
          <div class="companies__outer--box">
            <img src="../../assets/img/uph-logo.png" alt="uph-logo">
          </div>
          <div class="companies__outer--box">
            <img src="../../assets/img/bank-indonesia-logo.png" alt="bi-logo">
          </div>
          <div class="companies__outer--box">
            <img src="../../assets/img/binar-academy-logo.png" alt="binar-logo">
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Mitra',
};
</script>

<style lang="scss">
.mitra {
  text-align: center;
}

.companies__outer {
  display: flex;
  flex-wrap: wrap;
}

.companies__outer--box {
  margin-left: 0;
  margin-top: 40px;
  width: 33%;
}
</style>
