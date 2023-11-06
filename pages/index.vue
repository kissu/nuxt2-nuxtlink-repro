<template>
  <div>
    <NuxtLink to="/calculators">go to calculators</NuxtLink>
    <br />
    <br />
    <nuxt-link v-slot="{ route, navigate }" to="/calculators" custom>
      <a :href="'https://nuxt2-nuxtlink-repro.netlify.app' + '/calculators'" @click="navigate">
        Go to {{ route.fullPath }}
      </a>
      <a @click="navigate">Go to {{ route.fullPath }} (different way)</a>
    </nuxt-link>
  </div>
</template>

<script>
export default {
  name: 'IndexPage',
}
</script>
