<template>
<section class="section content narrower">
<h2 class="subtitle">
  {{ $t('contact tagline') }}
</h2>

<h3 class="strong">{{ $t('contact emails') }}</h3>
<p>
  {{ $t('contact sales') }}: <a href="mailto:sales@cg-wire.com">sales@cg-wire.com</a>
</p>
<p>
  {{ $t('contact support') }}: <a href="mailto:support@cg-wire.com">support@cg-wire.com</a>
</p>

<h3 class="strong">{{ $t('contact address') }}</h3>
<p>
CGWire<br>
84 avenue de la République<br>
75011 Paris<br>
France
</p>

<h3 class="strong">{{ $t('contact company identifier') }}</h3>
<p>
N° RCS: Paris 831 995 303
</p>
</section>

<Trial class="mt4" :cta="false" />
</template>

<script setup>
const name = 'Contact'
const { t } = useI18n()
useHead({
  title: 'CGWire | ' + t('footers link contact'),
  meta: buildPageMeta(
    t,
    'contact tagline',
    'contact tagline',
    'contact',
    'assets/images/logo.png'
  )
})
</script>
