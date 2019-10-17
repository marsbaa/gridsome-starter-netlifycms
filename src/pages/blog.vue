<template>
  <Layout>
    <h1>Hello</h1>
    <template>{{$page.posts}}</template>
  </Layout>
</template>

<page-query>
query Blog {
  posts: allPost {
    edges {
      node{
        id
        title
      }
    }
  }
}
</page-query>