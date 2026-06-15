<template>
  <section class="hero">
    <p class="eyebrow">Editorial / Nuxt Practice</p>
    <h1>
      IVE
      <span>ACCENDIO</span>
    </h1>
    <p class="subtitle">
      An editorial review of IVE's otherworldly ACCENDIO — a cinematic spell
      of mirror light, beauty, and quiet control.
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
  color: #c9b18d;
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
  color: #f2e6d2;
  font-size: clamp(64px, 13vw, 164px);
  line-height: 0.85;
  letter-spacing: -0.08em;
}

h1 span {
  display: block;
  color: #c39a68;
  font-style: italic;
}

.subtitle {
  max-width: 760px;
  margin: 40px 0 0;
  color: #d3c0af;
  font-size: clamp(20px, 3vw, 30px);
  line-height: 1.55;
}

.meta {
  display: flex;
  gap: 16px;
  flex-wrap: wrap;
  margin-top: 40px;
  color: #b9a08a;
  font-size: 14px;
  letter-spacing: 0.08em;
  text-transform: uppercase;
}

.meta p {
  margin: 0;
  padding: 10px 16px;
  border: 1px solid rgba(201, 177, 141, 0.28);
  border-radius: 999px;
  background: rgba(49, 30, 35, 0.32);
}
</style>
