<template>
  <div class="flex column">
    <div class="flex items-center nowrap">
        <div class="row-accent"></div>
        <p class="text-primary title-section">{{title}}</p>
    </div>
    <div>
        <p class="text-primary subtitle-section">{{subtitle}}</p>
    </div>
  </div>
</template>

<script>
export default {
    name: 'SectionTitle',
    props: {
        title: String,
        subtitle: String
    }
}
</script>

<style>

</style>