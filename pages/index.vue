<template>
  <section class="container">
    <div>
      <logo/>
      <p class="subtitle">
        {{ randomQuote }}
      </p>
    </div>
  </section>
</template>

<script>
import Logo from '~/components/Logo.vue'

export default {
  components: {
    Logo
  },
  data: function () {
    return {
      quotes: [`Snart är vi i land`,
        `Hamna inte snett nu`,
        `Vi kommer ro hem det här`]
    }
  },
  computed: {
    randomQuote: function () {
      return this.quotes[Math.floor(Math.random() * this.quotes.length)]
    }
  }
}
</script>

<style>
.container {
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif; /* 1 */
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 400;
  font-style: italic;
  font-size: 24pt;
  font-family: "Lato", sans-serif;
  color: #4d4d4c;
  word-spacing: 5px;
  padding: 15px 0px;
  background-color: #fff;
  margin: 30px 0px;
  padding: 15px 15px;
  max-width: 90vw;
}

.links {
  padding-top: 15px;
}
</style>
