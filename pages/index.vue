<template>
  <div>
    <NuxtLink to="/calculators">go to calculators</NuxtLink>
    <br />
    <NuxtLink :to="{ name: 'calculators' }">other way to go there</NuxtLink>
  </div>
</template>

<script>
export default {
  name: 'IndexPage',
}
</script>
