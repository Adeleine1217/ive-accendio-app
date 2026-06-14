<template>
  <section class="hero">
    <p class="eyebrow">K-pop Review / Nuxt Practice</p>
    <h1>
      IVE
      <span>REBEL HEART</span>
    </h1>
    <p class="subtitle">
      My first Nuxt page, written for a song that makes confidence feel
      elegant, emotional, and luminous.
    </p>
    <div class="meta">
      <p>Written by Adeleine Wang</p>
      <p>Built with Nuxt</p>
    </div>
  </section>
</template>

<style scoped>
.eyebrow {
  margin: 0 0 20px;
  color: #9a6d51;
  font-size: 12px;
  letter-spacing: 0.22em;
  text-transform: uppercase;
}

.hero {
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  padding: 48px clamp(24px, 6vw, 80px);
}

h1 {
  margin: 0;
  color: #1f1715;
  font-size: clamp(64px, 13vw, 164px);
  line-height: 0.85;
  letter-spacing: -0.08em;
}

h1 span {
  display: block;
  color: #8f5238;
  font-style: italic;
}

.subtitle {
  max-width: 760px;
  margin: 40px 0 0;
  color: #5d453c;
  font-size: clamp(20px, 3vw, 30px);
  line-height: 1.55;
}

.meta {
  display: flex;
  gap: 16px;
  flex-wrap: wrap;
  margin-top: 40px;
  color: #7c5c4d;
  font-size: 14px;
  letter-spacing: 0.08em;
  text-transform: uppercase;
}

.meta p {
  margin: 0;
  padding: 10px 16px;
  border: 1px solid rgba(124, 92, 77, 0.28);
  border-radius: 999px;
  background: rgba(255, 255, 255, 0.28);
}
</style>
