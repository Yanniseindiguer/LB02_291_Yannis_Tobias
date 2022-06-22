<template>
  <div class="about">
    <h1>Partnership </h1>
    <!--
  Vue Directives: Basic Directives (v-text, v-once, v-html, v-bind, v-if, v-show)
  -->
    <div>
      <h2 v-if="true" v-text="text">Wait..</h2>

      <h3 v-if="true" v-html="html">Wait..</h3>
      <h3 v-else-if="true" v-html="html">Wait..</h3>
      <a
          v-if="true"
          :href="link.url"
          :target="link.target"
          :tabindex="link.tabindex"
          v-text="link.title"
      />
    </div>

  </div>
</template>


<script>
export default {
  data() {
    return {
      // v-text
      text: 'Das ist Zara unser Sponsor.',
      // v-html
      html: 'Bei weiterer Interesse übere Zara kommt Ihr über den Link zu Ihrer Webseite.',
      // v-bind
      link: {
        url: 'https://www.zara.com/ch/',
        target: '_blank',
        tabindex: '0',
        title: 'Hier geht es zur offiziellen Zara Webseite',
      },
    }
  },
}

</script>