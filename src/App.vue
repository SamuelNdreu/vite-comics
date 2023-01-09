<script >
import DcHeader from './components/DcHeader.vue';
import DcMain from './components/DcMain.vue';
import DcFooter from './components/DcFooter.vue';

export default {
  components: {
    DcHeader,
    DcMain,
    DcFooter,
  }
}

</script>

<template>

  <header>
    <DcHeader />
  </header>

  <main>
    <DcMain />
  </main>

  <footer>
    <DcFooter />
  </footer>

</template>

<style >
.container {
  width: 80%;
  height: 100%;
  display: flex;
  margin: 0 auto;
  justify-content: space-between;
  align-items: center;
}
</style>


