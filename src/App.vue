<template>
  <div class="container">
    <div class="row">
      <div class="col-xs-12 col-sm-8 col-sm-offset-2 col-md-6 col-md-offset-3">
        <h1>Vuex</h1>
        <!--<app-result :counter="counter"></app-result>-->
        <!--<app-counter @updated="counter += $event"></app-counter>-->
        <app-result></app-result>
        <app-another-result></app-another-result>
        <app-counter></app-counter>
      </div>
    </div>
  </div>

</template>

<script>
  import Counter from './components/Counter.vue';
  import Result from './components/Result.vue';
  import AnotherResult from './components/AnotherResult.vue';
  export default {
    components: {
      appCounter: Counter,
      appResult: Result,
      appAnotherResult: AnotherResult
    },
    data() {
      return {
        counter: 0
      }
    }
  }
</script>

<style>

</style>