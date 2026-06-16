<script setup>
const siteUrl = 'https://ive-accendio-app.vercel.app'
const ogImage = `${siteUrl}/og-accendio.png`
const description =
  "A cultural review of IVE's ACCENDIO — exploring enchantment, illusion, and the cinematic architecture of a dark-fantasy K-pop moment."

useSeoMeta({
  // Core
  title: 'IVE — ACCENDIO Review | Adeleine Wang',
  description,

  // Open Graph
  ogTitle: 'IVE — ACCENDIO Review | Adeleine Wang',
  ogDescription: description,
  ogType: 'website',
  ogUrl: `${siteUrl}/`,
  ogSiteName: 'IVE ACCENDIO Review',
  ogImage,
  ogImageWidth: 1200,
  ogImageHeight: 630,
  ogImageAlt: 'IVE ACCENDIO — a cultural review by Adeleine Wang',

  // Twitter
  twitterCard: 'summary_large_image',
  twitterTitle: 'IVE — ACCENDIO Review | Adeleine Wang',
  twitterDescription: description,
  twitterImage: ogImage,
  twitterImageAlt: 'IVE ACCENDIO — a cultural review by Adeleine Wang',
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

<style scoped>
.site {
  min-height: 100vh;
  background:
    radial-gradient(circle at top left, rgba(255, 235, 205, 0.12), transparent 22%),
    linear-gradient(135deg, #12070f 0%, #291722 42%, #090407 100%);
  color: #f1e6d8;
  font-family: Georgia, 'Times New Roman', serif;
}
</style>
