<script setup>
import { useCounterStore } from "~/stores/myStore";

// access the `store` variable anywhere in the component ✨
//const { increment, doubleCount, count } = useCounterStore();

const counter = useCounterStore();

//console.log(increment);
</script>

<template>
  <div>
    Counter: {{ counter.count }} Counter: {{ counter.doubleCount }}
    <button @click="counter.increment">+</button>
    <button @click="counter.increment">-</button>

    <!--Counter id="counter"></Counter-->
  </div>
</template>
