<template>
  <div>
    <NuxtLink to="/calculators">go to calculators</NuxtLink>
    <br />
    <br />
    <nuxt-link v-slot="{ route, navigate }" to="/about" custom>
      <a @click="navigate">Go to {{ route.fullPath }} (non-working)</a>
      <a :href="'https://nuxt2-nuxtlink-repro.netlify.app' + '/about'" @click="navigate">
        Go to {{ route.fullPath }}
      </a>
    </nuxt-link>
  </div>
</template>

<script>
export default {
  name: 'IndexPage',
}
</script>
