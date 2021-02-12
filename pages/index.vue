<template>
  <section class="py-5 front-banner">
    <b-container class="py-lg-5">
      <b-row class="g-0">
        <div class="order-1 col-lg-6 order-lg-1">
          <h1>Hello, i am Yanuar Aditia.</h1>
          <p>I am an software developer and the backend team of <a href="//kiriminaja.com">KiriminAja.com</a>.
            Sometimes my work is open source and publicly available on github.
            You can follow me at <a href="//t.me/yanuaraditia">Telegram</a> where I mostly learning about backend technology.
          </p>
          <p>Outside of programming and creating new features, I enjoy video games, boba tea and customize my phone</p>
          <nuxt-link class="btn btn-primary btn-lg" to="/me">
            <svg xmlns="http://www.w3.org/2000/svg" class="icon" width="24" height="24" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><circle cx="12" cy="7" r="4" /><path d="M6 21v-2a4 4 0 0 1 4 -4h4a4 4 0 0 1 4 4v2" /></svg>
            About Me
          </nuxt-link>
          <a class="btn btn-link btn-lg" href="//t.me/yanuaraditia">
            <svg xmlns="http://www.w3.org/2000/svg" class="icon" width="24" height="24" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M15 10l-4 4l6 6l4 -16l-18 7l4 2l2 6l3 -4" /></svg>
            <span class="d-none d-lg-inline">Call me maybe</span>
          </a>
        </div>
        <div class="order-0 col-lg-auto order-lg-0">
          <div class="mb-5 mb-lg-0">
            <img src="~/assets/me.jpg" alt="" class="radius-100 img-fluid">
          </div>
        </div>
      </b-row>
    </b-container>
  </section>
</template>
<style lang="scss" scoped>
.front-banner {
  @media screen and (min-width: 1024px) {
    h1 {
      font-size: 3rem;
    }
    img {
      max-width: 80%;
    }
    p {
      font-size: 1.4rem;
    }
  }
  @media screen and (max-width: 1023px) {
    img {
      max-width: 50%;
      height: auto;
    }
  }
}
</style>
<script>
export default {
  head: {
    title: 'Home'
  }
}
</script>
