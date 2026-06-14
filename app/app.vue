<script setup>
const siteUrl = 'https://ive-rebel-heart.vercel.app'
const ogImage = `${siteUrl}/og-rebel-heart.png`
const description =
  "A cultural review of IVE's REBEL HEART — exploring confidence, girlhood, and the emotional architecture of a defining K-pop moment."

useSeoMeta({
  // Core
  title: 'IVE — REBEL HEART Review | Adeleine Wang',
  description,

  // Open Graph
  ogTitle: 'IVE — REBEL HEART Review | Adeleine Wang',
  ogDescription: description,
  ogType: 'website',
  ogUrl: `${siteUrl}/`,
  ogSiteName: 'IVE REBEL HEART Review',
  ogImage,
  ogImageWidth: 1200,
  ogImageHeight: 630,
  ogImageAlt: 'IVE REBEL HEART — a cultural review by Adeleine Wang',

  // Twitter
  twitterCard: 'summary_large_image',
  twitterTitle: 'IVE — REBEL HEART Review | Adeleine Wang',
  twitterDescription: description,
  twitterImage: ogImage,
  twitterImageAlt: 'IVE REBEL HEART — a cultural review by Adeleine Wang',
})

useHead({
  link: [{ rel: 'canonical', href: `${siteUrl}/` }],
})
</script>

<template>
  <div class="site">
    <HeroSection />
    <SongIntro />
    <MVSection />
    <MemberGrid />
    <ThemeAnalysis />
    <FooterSection />
  </div>
</template>

<style>
*,
*::before,
*::after {
  box-sizing: border-box;
}
</style>

<style scoped>
.site {
  min-height: 100vh;
  background:
    radial-gradient(circle at top left, rgba(255, 255, 255, 0.9), transparent 32%),
    linear-gradient(135deg, #f7efe8 0%, #efe0d6 48%, #d8bfae 100%);
  color: #241915;
  font-family: Georgia, 'Times New Roman', serif;
}
</style>
