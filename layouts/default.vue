<template>
  <div>
    <!-- <tm-top-banner /> -->
    <nuxt />
    <tm-footer />
  </div>
</template>

<script>
import TmFooter from '~/components/TmFooter.vue'
// import TmTopBanner from '~/components/TmTopBanner.vue'

export default {
  components: {
    TmFooter,
    // TmTopBanner,
  },
}
</script>

<style lang="stylus">
// Accessible/SEO friendly CSS hiding
.sr-only
  position absolute
  height 1px
  width 1px
  overflow hidden
  clip rect(1px, 1px, 1px, 1px)

.section-container
  position relative
  max-width 96rem
  margin 0 auto
  .container
    display grid
    grid-template-columns repeat(12, 1fr)
    gap 0 2rem
    max-width var(--container-mw-lg)
    margin 0 auto

.section
  overflow hidden
  position relative
  padding-top 6rem
  padding-bottom 6rem

.section-header
  padding-top 1rem
  min-height 3rem
  color var(--gray-600)
  border-top 1px solid #282B53

.section-title
  color var(--white)

@media screen and (max-width: 1279px)
  .section
    padding-top 6rem
    padding-bottom 6rem

@media screen and (max-width: 1024px)
  .section
    padding-top 4rem
    padding-bottom 4rem
  .section-container
    .container
      gap 0 1.5rem

@media screen and (max-width: 767px)
  .section-container
    padding-top 1.5rem
    .container
      gap 0 1rem

@media screen and (min-width: 1920px)
  .section
    padding-top 8rem
    padding-bottom 8rem
</style>
