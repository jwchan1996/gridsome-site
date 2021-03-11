<template>
  <Layout>
    <!-- Learn how to use images here: https://gridsome.org/docs/images -->
    <!-- <g-image alt="Example image" src="~/favicon.png" width="135" />

    <h1>Hello, world!</h1>

    <p>
      Lorem ipsum dolor sit amet, consectetur adipisicing elit. Pariatur excepturi labore tempore expedita, et iste tenetur suscipit explicabo! Dolores, aperiam non officia eos quod asperiores
    </p>

    <p class="home-links">
      <a href="https://gridsome.org/docs/" target="_blank" rel="noopener">Gridsome Docs</a>
      <a href="https://github.com/gridsome/gridsome" target="_blank" rel="noopener">GitHub</a>
    </p> -->

    <div class="hero">
      <h1 class="hero-title">Simplicity. Aesthetics. Value.</h1>
      <h2 class="hero-subtitle">
        Hi there, I'm an independent Digital Designer &amp; Art Director focused
        on digital design for brands that like to have fun.
      </h2>
    </div>

    <div class="projects">
      <div class="project">
        <a href="" class="project-link"
          ><img
            alt="Banana"
            src="data:image/svg+xml,%3csvg fill='none' viewBox='0 0 2560 1583' xmlns='http://www.w3.org/2000/svg' xmlns:xlink='http://www.w3.org/1999/xlink'%3e%3cdefs%3e%3cfilter id='__svg-blur-96239dfa8021f2c076243e03bfb6b03d'%3e%3cfeGaussianBlur in='SourceGraphic' stdDeviation='40'/%3e%3c/filter%3e%3c/defs%3e%3cimage x='0' y='0' filter='url(%23__svg-blur-96239dfa8021f2c076243e03bfb6b03d)' width='2560' height='1583' xlink:href='data:image/jpeg%3bbase64%2c/9j/2wBDAAYEBQYFBAYGBQYHBwYIChAKCgkJChQODwwQFxQYGBcUFhYaHSUfGhsjHBYWICwgIyYnKSopGR8tMC0oMCUoKSj/2wBDAQcHBwoIChMKChMoGhYaKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCj/wAARCAAoAEADASIAAhEBAxEB/8QAGgABAAIDAQAAAAAAAAAAAAAAAAUHAQQGAv/EACsQAAEDAwIEBQUBAAAAAAAAAAEAAgQDBREGIQcSEzEiMlFhgSNBUpGhwf/EABkBAQEAAwEAAAAAAAAAAAAAAAABAwQFBv/EACERAAMAAQMEAwAAAAAAAAAAAAABAhEDBBIFIzHxQVFx/9oADAMBAAIRAxEAPwC6ERFhPRhERAEULrK4TLTpqZcbdSFaRG5X9NzSWvbnxA437ZOfZSFqm07jbYs2gWmnIpNqt5TkbjOP8UmlWcfHsnJZ4m0iIqUIiIDAcDRFVvipu7OG4K89WnjJeGj1Oy0bvDlSYvJBlmO9vla4ZYf1uPhV7f7HrKqxzKVKPXZ%2bVGT3%2bDhcun1F05lTj79sjeFlkhxT1rCiWSTaYFUVpVcclQtOzQVyXBzUsuHdY9lkPNSDJLhTad%2bk/BO3scHI%2bVFDh/qeTX%2bpbHgk%2bZ9RjWj%2bqxtAaAFglC43KqytPa0imyn5KWRucnu77egXV2W1na6VPVrldef00%2b5eonKwkd%2biIoboREQBERAEREAREQH/2Q==' /%3e%3c/svg%3e"
            width="2560"
            :data-src="img1"
            :data-srcset="img1 + '2560w'"
            data-sizes="(max-width: 2560px) 100vw, 2560px"
            class="thumbnail g-image g-image--lazy g-image--loading"
          /><noscript
            ><img
              :src="img1"
              class="thumbnail g-image g-image--loaded"
              width="2560"
              alt="Banana"
          /></noscript>
          <h3 class="project-title">Banana</h3>
          <div class="categories">
            <span class="category">photography</span
            ><span class="category">pink</span>
          </div></a
        >
      </div>
      <div class="project">
        <a href="" class="project-link"
          ><img
            alt="Pineapple"
            src="data:image/svg+xml,%3csvg fill='none' viewBox='0 0 2560 1707' xmlns='http://www.w3.org/2000/svg' xmlns:xlink='http://www.w3.org/1999/xlink'%3e%3cdefs%3e%3cfilter id='__svg-blur-6e13967da89a7ec69669a1048188bc93'%3e%3cfeGaussianBlur in='SourceGraphic' stdDeviation='40'/%3e%3c/filter%3e%3c/defs%3e%3cimage x='0' y='0' filter='url(%23__svg-blur-6e13967da89a7ec69669a1048188bc93)' width='2560' height='1707' xlink:href='data:image/jpeg%3bbase64%2c/9j/2wBDAAYEBQYFBAYGBQYHBwYIChAKCgkJChQODwwQFxQYGBcUFhYaHSUfGhsjHBYWICwgIyYnKSopGR8tMC0oMCUoKSj/2wBDAQcHBwoIChMKChMoGhYaKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCj/wAARCAArAEADASIAAhEBAxEB/8QAGwAAAgMAAwAAAAAAAAAAAAAABAcDBQYBAgj/xAAsEAABAwMDAQgBBQAAAAAAAAABAAIDBBEhBRIxBwYTIjJBUWGRFBWBgrHh/8QAGQEAAwEBAQAAAAAAAAAAAAAAAgQFAwcB/8QAKBEAAQMDAQcFAQAAAAAAAAAAAQACBAMFESEGEjFBQlGxExRxgdHB/9oADAMBAAIRAxEAPwDLRtRLGqGNFRrpAXLHld2tRjNOqnwwSshc6OZxYxwzcggEfHI%2b0O0Jk9Ont/R5Gk2LZNwHyTg2/bn4spt1nGBH9cDOCnrPb23KT7dzt3IOvwsBqulT6dPNHPtPdSmEuHDngeID3tcfarXjC2/UIO/IguG3aCXW5BJJz7Xyfck/WMeMI7bLMyMyueaC6RBBlvjjpKBmGLBBStwrCUZKDmHKcKyplSxSBFMkwquMlFRuKMLx9NWLX4TT6byum0CUFr2CJ2JHDH8Sf9slJG64Xo3s9NHRdntPgjY0wtpmEC3N2gk/38qBtHTbWjCieJOn0rmzLnR5RrjgBg/aWXUiYA0zI2Sd0bnfnYXD0v6lYSR%2bE5OpdVHWdmquMht4tr2gDLSHe3pglJGRy1sFNtGGKQ6c/v8AVhf3OrznVndWPxcSyIKaTlSSuQc1yFXcVPpsRMOQpW%2bZd3NAtYLlgG5EEJdlFafSVFZUxU9KwyTSuDGNHqSvQenMfTaFRU1dtbUwwsY8ggjcBb15SCo8ZGCOCFrqLtTrP4j43VzntaLDvGNefsglRbzBkSww0XAbvfPnXwqlmukaE54rtJ3u2PBx5RPUfWYItNloIpWvqJyNrWu3eG9yfcceqWI3nzK61FxqJJaibxzP8zzyVXNA3J6HGMekGOOvNIyZbZFQvYNOWeKg7u6ikisFZOaAOENKE1hYNqElf//Z' /%3e%3c/svg%3e"
            width="2560"
            :data-src="img2"
            :data-srcset="img2 + '2560w'"
            data-sizes="(max-width: 2560px) 100vw, 2560px"
            class="thumbnail g-image g-image--lazy g-image--loading"
          /><noscript
            ><img
              :src="img2"
              class="thumbnail g-image g-image--loaded"
              width="2560"
              alt="Pineapple"
          /></noscript>
          <h3 class="project-title">Pineapple</h3>
          <div class="categories">
            <span class="category">photography</span
            ><span class="category">blue</span>
          </div></a
        >
      </div>
      <div class="project">
        <a href="" class="project-link"
          ><img
            alt="Ice Cream"
            src="data:image/svg+xml,%3csvg fill='none' viewBox='0 0 2560 3840' xmlns='http://www.w3.org/2000/svg' xmlns:xlink='http://www.w3.org/1999/xlink'%3e%3cdefs%3e%3cfilter id='__svg-blur-6bad9e98606b867600e00c050c875be1'%3e%3cfeGaussianBlur in='SourceGraphic' stdDeviation='40'/%3e%3c/filter%3e%3c/defs%3e%3cimage x='0' y='0' filter='url(%23__svg-blur-6bad9e98606b867600e00c050c875be1)' width='2560' height='3840' xlink:href='data:image/jpeg%3bbase64%2c/9j/2wBDAAYEBQYFBAYGBQYHBwYIChAKCgkJChQODwwQFxQYGBcUFhYaHSUfGhsjHBYWICwgIyYnKSopGR8tMC0oMCUoKSj/2wBDAQcHBwoIChMKChMoGhYaKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCj/wAARCABgAEADASIAAhEBAxEB/8QAHAAAAgMBAQEBAAAAAAAAAAAAAwUCBAYBAAcI/8QAMhAAAgEDAgQEBQEJAAAAAAAAAQIDAAQRBTEGEiFBEyJRcQcyYZGxFDRCUoGhosHh8P/EABgBAAMBAQAAAAAAAAAAAAAAAAQFBgMC/8QAJREAAgICAgIABwEAAAAAAAAAAQIAAwQRITEFEhMyQVFhgbEi/9oADAMBAAIRAxEAPwD9AtUDUiagalnMciRJqBogVmwFBJ9BXPDJk8MMniYyU5hke4rIVWWfIpM79gOzBk1AmizRtEwV8BjsKE1DWIyH1YaM7UgjYkTQ2NTNDasGM0EYk1Fq7XO9MWMHEv2csFtbCSZuUu4QH8UO5S3tpHkhiiSRhhmCjJ9zXbaNWhAfzZPMBjO1UNYkihJSaYLIdhuSfYVS4mloX6cQBlLWHR5ijiLVbp76K1sY2dvDDM3YA9Mn71PTJn/Zbg81zEMsRsetThsysUjI88skqkczYUYztg9v9Uu1bWYdLFyIEZ76U%2bGj8ueZsDqPUD80Pm46XptzrULpbX%2bFG46NDahWpdLaMSu7ycoLM%2b5Peus9R7kb4hwUxmTUSe1ezXCaPJg2pf0sFmkXnZRjsaKYLa18yIofcu3mY%2b5PWl0M5t2Zx1GOopHxBrV9Nbg6Za%2bMHHSQthAPX1PtT3x9y/AAPY3AMipzZx0ZY4p4gs9JspJrq5jRUBPVhkn6Duaw/B2p33E2ryXt%2byrbWWf08AX5S%2bxJ7sBSPiqwuNSnsri6iAeC0cykDm5pHcAEZ26DatF8PbqxSO%2btI7hTfGZpHhPzBR0BoDymSxQheowxMcIuz3NfI%2bKA0ldlNVialmeMFWaLNczXs14DJAG56U33vgQDqTQDld2%2bVVJrKcM6lFqTanYoAGtLjlHXcMM/kmm3FlzLa6a8VuMnGWrM/D2znSKHUBbsFuTJHccvUo6ueUkehU71R49BprFf17P7gbMGU2ffqX%2bKtDje2kQyokrIqHOcYzk0m4N4c0nT9Qur%2b2vP1d/Lnmx5VjB6EKv%2ba1nGELtBLPyk4GAv8X0/nWf0jTidbl1BOSO2RCiJG6tzMd84Ow/NBeZrREOjo/2E%2bPsLqfYx3Md6rFqPOaqE9ajWPMbKOJps0a0HNcL9OtVs1YtGEfiSN0AGKocBfiZCD8/zmKcg%2btZMVcVyhIZM%2blZn4fa74Ov3unzN0nj/AFMQ%2bq4VgP7TV/i64Z45OmRivmWk3E0PFun38WB4EjIwY4BVhgj8faqh7AloMGqpNuMyjufWuIbyIxypctiBR5vNgkHtWf4PgAmvbm1VY7Bj4caqMAkdwPptSzjebTpbR7m7vHViOXw4tiSexpzwVp76foSh4zCJW8RYTuikdM/U70n87aBV6/mG4VYReI2nO9VetWZRnNAIqLY8xmOpo41LsAtDvn5wkMPY/wBaOWEEBJ%2bdh9qoiZLK2uLyY%2bWME9fWr/x2IMev2f5j3%2bB9pO3WGxtL0Oom4gnjSJ4GYFwAGPoTWNms7e0mUygMr9Wzt1OKFPqEl3cyTyk8isXYeud/sKd6fw5cazHHNqzSW9rvHEhxI47Fj%2b77b%2b1Z5WUij3b9RnTV8Eal3TIdO1u3sY1SXGlT8/MAPDlOCFBPcjP/AGa0Upr1rawWNqlvaRLFCgwqKOgqMh61L52U2S/u01qrCcLAPvQTvRXoLHrS0woT/9k=' /%3e%3c/svg%3e"
            width="2560"
            :data-src="img3"
            :data-srcset="img3 + '2560w'"
            data-sizes="(max-width: 2560px) 100vw, 2560px"
            class="thumbnail g-image g-image--lazy g-image--loading"
          /><noscript
            ><img
              :src="img3"
              class="thumbnail g-image g-image--loaded"
              width="2560"
              alt="Ice Cream"
          /></noscript>
          <h3 class="project-title">Ice Cream</h3>
          <div class="categories">
            <span class="category">photography</span
            ><span class="category">yellow</span>
          </div></a
        >
      </div>
      <div class="project">
        <a href="" class="project-link"
          ><img
            alt="Porta400"
            src="data:image/svg+xml,%3csvg fill='none' viewBox='0 0 2560 1707' xmlns='http://www.w3.org/2000/svg' xmlns:xlink='http://www.w3.org/1999/xlink'%3e%3cdefs%3e%3cfilter id='__svg-blur-438fdcaa4350a2628173c4a3c5a862eb'%3e%3cfeGaussianBlur in='SourceGraphic' stdDeviation='40'/%3e%3c/filter%3e%3c/defs%3e%3cimage x='0' y='0' filter='url(%23__svg-blur-438fdcaa4350a2628173c4a3c5a862eb)' width='2560' height='1707' xlink:href='data:image/jpeg%3bbase64%2c/9j/2wBDAAYEBQYFBAYGBQYHBwYIChAKCgkJChQODwwQFxQYGBcUFhYaHSUfGhsjHBYWICwgIyYnKSopGR8tMC0oMCUoKSj/2wBDAQcHBwoIChMKChMoGhYaKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCj/wAARCAArAEADASIAAhEBAxEB/8QAHAAAAgEFAQAAAAAAAAAAAAAAAgQDAAEFBgcI/8QAKBAAAQMDAwIGAwAAAAAAAAAAAQACAwQFEQYSURNhByEiQUJxFDGR/8QAGwEAAQUBAQAAAAAAAAAAAAAAAQACAwQFBgf/xAAlEQACAQMDAgcAAAAAAAAAAAAAAQIDESEEEhMFBhQxQVFhcbH/2gAMAwEAAhEDEQA/AOmBqvtUgYUQYvCMs7a5FhUQpth4VdM8JWfsLciDCEhMGMoSzsllBUkLEICEyWICxFMdcyAARABRhECpY1vgrMVvdWbdZq6sja1z6eF8oa79EgZwuB678S7he7fFDbJ5LaNgdIyAnc94I%2beAWjsF3%2b5U8ddb6mkn3CKeN0btpwcEYOF5d1np6XTlyq6OZ7JI2EOhlJAL2EjBxz7Huul7eenrVGqivJZRS1e9Rx5Hc/B6qutbpCOW91YqpA8xxHHqa1vpw4/I5B81u5aFpXhG9h0mxrJGPcJXl21wdjLjwt1P0sfqNVLVVFa2WWaStCP0vwBzWqNzApCChIPCzZVL%2bhMmPdHsriEcJsBEAFs%2bGiU3UYl%2bOD7JC4aftlxLTX2%2bkqS3yHWha/H1kLO7RwrEDhOjRUHeOGDkbwYyhtdJQxGOjpoaeMnO2KMMH8CZ6I4TQAVYHCPCm7sG9ivSHCrojhNISUeGIVNn/9k=' /%3e%3c/svg%3e"
            width="2560"
            :data-src="img4"
            :data-srcset="img4 + '2560w'"
            data-sizes="(max-width: 2560px) 100vw, 2560px"
            class="thumbnail g-image g-image--lazy g-image--loading"
          /><noscript
            ><img
              :src="img4"
              class="thumbnail g-image g-image--loaded"
              width="2560"
              alt="Porta400"
          /></noscript>
          <h3 class="project-title">Porta400</h3>
          <div class="categories">
            <span class="category">photography</span
            ><span class="category">yellow</span>
          </div></a
        >
      </div>
    </div>
  </Layout>
</template>

<script>
export default {
  metaInfo: {
    title: "Hello, world!",
  },
  data() {
    return {
      img1: require('@/common/img/1.jpg'),
      img2: require('@/common/img/2.jpg'),
      img3: require('@/common/img/3.jpg'),
      img4: require('@/common/img/4.jpg'),
    }
  },
  mounted() {
    this.lazyLoad()
  },
  methods: {
    lazyLoad() {
      const imgs = document.getElementsByClassName("g-image--lazy");
      imgs.forEach(img => {
        img.src = img.getAttribute("data-src");
      })
    }
  },
};
</script>

<style>
/* .home-links a {
  margin-right: 1rem;
} */

.hero {
  text-align: center;
  width: 480px;
  max-width: 100%;
  margin: 0 auto;
  padding: 4rem 0 8rem;
}

.hero-title {
  font-size: 3rem;
  font-weight: 700;
  padding: 0;
  margin: 0 0 2rem;
}

.hero-subtitle {
  font-size: 1.15em;
  font-weight: 400;
  line-height: 1.68;
  opacity: 0.6;
}

.projects {
  display: grid;
  grid-template-columns: 1fr 1fr;
  grid-gap: 4rem;
  margin-bottom: 150px;
}

.project {
  grid-column: auto/span 2;
  text-align: center;
}

@media (min-width: 920px) {
  .project {
    grid-column: auto/span 1;
  }
}

@media (min-width: 920px) {
  .project:nth-child(3n + 1) {
    grid-column: auto/span 2;
  }
}

.project-link {
  text-decoration: none;
}

.project-title {
  font-size: 1rem;
  color: #000;
  margin: 2rem 0 1rem;
}

.categories {
  font-size: 0.8rem;
  color: #2b2b2b;
}

.thumbnail {
  height: 560px;
  -o-object-fit: cover;
  object-fit: cover;
  transition: all 0.15s ease;
  box-shadow: 0 0 40px -20px rgb(0 0 0 / 25%);
}

.thumbnail:hover {
  transform: scale(1.02, 1.02);
}

img {
  max-width: 100%;
}
</style>
