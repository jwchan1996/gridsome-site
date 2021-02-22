<template>
  <Layout>
    <div>
      <h1>Posts2</h1>
      <ul>
        <li v-for="edge in $page.posts.edges" :key="edge.node.id">
          <g-link :to="edge.node.path">{{ edge.node.title }}</g-link>
        </li>
      </ul>
    </div>
  </Layout>
</template>

<page-query>
query {
  posts: allPost {
    edges {
      node {
        id
        title
        path
      }
    }
  }
}
</page-query>

<script>
export default {

}
</script>

<style>
.pager .active {
  color: #fff;
  background-color: #007bff;
  border-color: #007bff;
}

.pager .page-link {
  display: inline;
}
</style>
