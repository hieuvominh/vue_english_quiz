<template>
  <Layout>
    <Header><index /></Header>
    <Layout>
      <Content> <articles /></Content>
    </Layout>
  </Layout>
</template>

<script>
import Index from '~/components/Index.vue'
import Articles from '~/components/Articles.vue'
import 'ant-design-vue/dist/antd.css'


export default {
  components: {
    Index,
    Articles
  }
}
</script>

<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
