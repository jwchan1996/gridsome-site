<template>
  <div class="layout">
    <header class="header">
      <div class="header-container">
        <strong>
          <!-- <g-link to="/">{{ $static.metadata.siteName }}</g-link> -->
          <g-link to="/">
            <img class="logo" src="@/common/img/logo.svg" alt="">
          </g-link>
        </strong>
        <nav class="nav">
          <g-link class="nav__link" to="/">Home</g-link>
          <g-link class="nav__link" to="/about/">About</g-link>
          <!-- <g-link class="nav__link" to="/posts1/">Posts1</g-link>
          <g-link class="nav__link" to="/posts2/">Posts2</g-link> -->
        </nav>
      </div>
    </header>
    <div class="container">
      <slot/>
    </div>
  </div>
</template>

<static-query>
query {
  metadata {
    siteName
  }
}
</static-query>

<style>
* {
  box-sizing: border-box;
}

body {
  font-family: -apple-system,system-ui,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica Neue,Arial,sans-serif;
  margin:0;
  padding:0;
  line-height: 1.5;
}

.layout {
  margin: 0 auto;
  padding-left: 20px;
  padding-right: 20px;
  padding: 6rem 0 0;
}

@media (min-width: 860px) {
  .header-container, .container {
    padding: 0 6rem !important;
  }
}

.container {
  max-width: 1200px;
  padding: 6rem 2rem 0;
  margin: 0 auto;
}

.header {
  z-index: 10;
  position: fixed;
  width: 100%;
  top: 0;
  left: 0;
}

@media (min-width: 860px) {
  .header-container {
      padding: 0 6rem;
  }
}

.header-container {
  display: flex;
  max-width: 1200px;
  margin: 0 auto;
  justify-content: space-between;
  align-items: center;
  width: 100%;
  height: 6rem;
  padding: 0 2rem;
}

.header .logo {
  height: 1.5rem;
}

.nav__link {
  /* margin-left: 20px; */
  font-size: .9rem;
  font-weight: 600;
  text-decoration: none;
  margin-top: 4px;
  margin-left: 2rem;
  padding-bottom: 4px;
  border-bottom: 1px solid;
  border-color: transparent;
  transition: border .15s;
}
</style>
