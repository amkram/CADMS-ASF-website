<template>
  <footer class="site-footer">
    CADMS &nbsp; | &nbsp; Univeristy of California, Davis &copy; {{ new Date().getFullYear() }}
    <br />
  </footer>
</template>

<script>
export default {
  name: 'SiteFooter'
}
</script>

<style scoped>
footer {
  background: #eee;
  padding: 20px 10px;
  text-align: center;
  transition: 0.5s ease all;
}
</style>
