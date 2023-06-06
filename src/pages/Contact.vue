<template>
  <Layout>
    <h1>Get in touch</h1>
    <form
  action="https://formspree.io/f/xqkovdgo"
  method="POST">
      <label>
        Your name:
        <input type="text" name="name">
      </label>
      <label>
        Your email:
        <input type="email" name="email">
      </label>
      <label>
        Your message:
        <textarea name="message"></textarea>
      </label>
      <button type="submit">Send</button>
    </form>

<p class="social-links">
      <a href="https://www.linkedin.com/in/maggie-cameron-877b82106/?originalSubdomain=uk" target="_blank" rel="noopener">LinkedIn</a>
      <a href="https://github.com/SirDegrid" target="_blank" rel="noopener">GitHub</a>
    </p>

  </Layout>
</template>

<script>
export default {
  metaInfo: {
    title: 'Contact'
  }
}
</script>

<style>
.social-links a {
  margin-right: 1rem;
}
</style>