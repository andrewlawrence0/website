<template>
<div class="kitsu-page studio-database">

  <SolutionHeaderBlock
    page-key="studio-database"
  />

  <FeatureBlock
    section-key="studio-database"
    feature-key="boost"
    :shadow="false"
    colored
  />

  <FeatureBlock
    section-key="studio-database"
    feature-key="api"
    :shadow="false"
    reverted
  />

  <FeatureBlock
    section-key="studio-database"
    feature-key="python"
    colored
    gradient
  />

  <Trial />
</div>
</template>

<script setup>
const name = 'Team Collaboration'
const { t } = useI18n()
useHead({
  title: 'CGWire | Kitsu / ' + t('studio-database header tagline'),
  meta: buildPageMeta(
    t,
    'studio-database header tagline',
    'studio-database header explanation',
    'studio-database',
    'studio-database.0c519a6b.png'
  )
})
</script>
