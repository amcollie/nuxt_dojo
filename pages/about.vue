<template>
  <main>
    <h1>About Us</h1>
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Repellat at, numquam, dolores voluptas nihil ut reiciendis officia natus iste quasi laudantium, eos soluta sit accusantium et veniam a. Eligendi assumenda soluta repudiandae eum nisi, aliquid quas voluptates consequatur voluptate? Odio.</p>
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Repellat at, numquam, dolores voluptas nihil ut reiciendis officia natus iste quasi laudantium, eos soluta sit accusantium et veniam a. Eligendi assumenda soluta repudiandae eum nisi, aliquid quas voluptates consequatur voluptate? Odio.</p>
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Repellat at, numquam, dolores voluptas nihil ut reiciendis officia natus iste quasi laudantium, eos soluta sit accusantium et veniam a. Eligendi assumenda soluta repudiandae eum nisi, aliquid quas voluptates consequatur voluptate? Odio.</p>
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Repellat at, numquam, dolores voluptas nihil ut reiciendis officia natus iste quasi laudantium, eos soluta sit accusantium et veniam a. Eligendi assumenda soluta repudiandae eum nisi, aliquid quas voluptates consequatur voluptate? Odio.</p>
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Repellat at, numquam, dolores voluptas nihil ut reiciendis officia natus iste quasi laudantium, eos soluta sit accusantium et veniam a. Eligendi assumenda soluta repudiandae eum nisi, aliquid quas voluptates consequatur voluptate? Odio.</p>
    <pre>{{ data }}</pre>
  </main>
</template>

<script setup>
  const { data } = await useFetch('/api/currency/usd')
</script>

<style scoped>
  h1 {
    margin-bottom: 20px;
    font-size: 2rem;
  }
  p {
    margin: 20px 0;
  }
</style>    