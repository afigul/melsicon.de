<template>
    <section
        id="home"
        class="section section-home">
        <article class="article article-hero">
            <h1 class="main-heading">{{ $t('hero.heading') }}</h1>
            <p class="paragraph">{{ $t('hero.description') }}</p>
        </article>
        <illustration-hero/>
    </section>
</template>

<script>
import IllustrationHero from '@/components/graphics/illustrations/IllustrationHero'
export default {
  name: 'Home',
  components: {
    IllustrationHero
  }
}
</script>

<style lang="sass" scoped>

  .section-home
    flex-wrap: nowrap
    align-items: center
    padding-top: 3em
    @include small
      flex-wrap: wrap

  .main-heading
    font-size: 3em
    font-weight: 200
    letter-spacing: 1px
    margin-bottom: .3em
    @include medium
      font-size: 2.5em
    @include small
      margin-top: 1em
      font-size: 2.2em

</style>
