<template>
  <section class="song-intro">
    <div class="inner">
      <p class="eyebrow">The Song</p>
      <div class="intro-layout">
        <div class="intro-label">
          <h2 class="intro-title">ACCENDIO</h2>
          <p class="intro-release">IVE · 2024</p>
          <div class="intro-rule" />
        </div>
        <div class="intro-text">
          <p>
            ACCENDIO opens like a ritual: slow, shimmering synths that feel
            less like machinery and more like candlelight reflected in glass.
            The song is deliberately cinematic, a dark fantasy magnetised by
            image and intent.
          </p>
          <p>
            Its power is in the way it makes control feel luxurious. Every
            breath, every vocal shadow, is arranged as if it were part of a
            spell — not to conquer the listener, but to invite them into a
            space of elegant unease.
          </p>
          <p>
            IVE has always been meticulous with their image. Here, that
            meticulousness becomes a kind of magic. ACCENDIO is not just a
            song. It is a mirror chamber of beauty, illusion, and the fierce
            stillness that happens when looking at yourself in a new light.
          </p>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.eyebrow {
  margin: 0 0 20px;
  color: #d8b88d;
  font-size: 12px;
  letter-spacing: 0.22em;
  text-transform: uppercase;
}

.inner {
  max-width: 1200px;
  margin: 0 auto;
}

.song-intro {
  padding: 88px clamp(24px, 6vw, 80px) 104px;
  background: rgba(22, 14, 20, 0.88);
  border-top: 1px solid rgba(255, 209, 159, 0.12);
}

.intro-layout {
  display: grid;
  grid-template-columns: 260px 1fr;
  gap: 72px;
  align-items: start;
  margin-top: 32px;
}

.intro-title {
  margin: 0;
  color: #f2e5d2;
  font-size: clamp(36px, 5vw, 60px);
  line-height: 0.9;
  letter-spacing: -0.06em;
}

.intro-release {
  margin: 18px 0 0;
  color: #bb9b70;
  font-size: 13px;
  letter-spacing: 0.18em;
  text-transform: uppercase;
}

.intro-rule {
  width: 48px;
  height: 2px;
  background: #c39a68;
  margin-top: 28px;
}

.intro-text p {
  margin: 0 0 22px;
  color: #d8c8b8;
  font-size: 18px;
  line-height: 1.85;
}

.intro-text p:last-child {
  margin-bottom: 0;
}

@media (max-width: 960px) {
  .intro-layout {
    grid-template-columns: 1fr;
    gap: 36px;
  }
}
</style>
