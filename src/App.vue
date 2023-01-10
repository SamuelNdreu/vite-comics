<script >
import DcHeader from './components/DcHeader.vue';
import DcMain from './components/DcMain.vue';
import DcCards from './components/DcCards.vue';
import DcFooter from './components/DcFooter.vue';
import BlueBand from './components/BlueBand.vue';

export default {
  components: {
    DcHeader,
    DcMain,
    DcCards,
    DcFooter,
    BlueBand,
  }
}

</script>

<template>

  <header>
    <DcHeader />
  </header>

  <main>
    <DcMain />
    <DcCards />
    <BlueBand />
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


