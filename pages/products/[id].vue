<template>
  <Head>
    <Title>Nuxt Dojo | {{ product.title }}</Title>
    <Meta name="description" :content="product.description" />
  </Head>
  <main>
    <ProductDetail :product="product" />
  </main>
</template>

<script setup>
  definePageMeta({
    layout: 'products'
  })

  const { id } = useRoute().params
  const { data: product } = await useFetch(`https://fakestoreapi.com/products/${ id }`)
  if (!product.value) {
    throw createError({
      statusCode: 404,
      statusMessage: `Product with ID ${ id } not found`,
      fatal: true
    })
  }
</script>

<style scoped>
</style>