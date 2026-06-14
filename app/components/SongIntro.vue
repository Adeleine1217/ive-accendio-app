<template>
  <section class="song-intro">
    <div class="inner">
      <p class="eyebrow">The Song</p>
      <div class="intro-layout">
        <div class="intro-label">
          <h2 class="intro-title">REBEL<br>HEART</h2>
          <p class="intro-release">IVE · 2024</p>
          <div class="intro-rule" />
        </div>
        <div class="intro-text">
          <p>
            Released in 2024 as part of IVE's <em>IVE SWITCH</em> era,
            "REBEL HEART" stands apart from the group's signature polish.
            It is not a perfect pop confection — and that, precisely, is its
            power.
          </p>
          <p>
            The song opens with a restrained tension and builds into something
            deeply expressive: a layered pop record that balances vulnerability
            with defiance. It does not shout its rebellion. Instead, it
            whispers it — which is far more arresting.
          </p>
          <p>
            What makes "REBEL HEART" worth writing about is the emotional
            intelligence behind it. IVE has always been associated with a cool,
            aspirational image. Here, they let something softer and stranger
            through — and the result feels like a defining moment.
          </p>
        </div>
      </div>
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

.inner {
  max-width: 1200px;
  margin: 0 auto;
}

.song-intro {
  padding: 88px clamp(24px, 6vw, 80px) 104px;
  background: rgba(255, 250, 246, 0.6);
  border-top: 1px solid rgba(124, 92, 77, 0.14);
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
  color: #1f1715;
  font-size: clamp(36px, 5vw, 60px);
  line-height: 0.9;
  letter-spacing: -0.06em;
}

.intro-release {
  margin: 18px 0 0;
  color: #a06f52;
  font-size: 13px;
  letter-spacing: 0.18em;
  text-transform: uppercase;
}

.intro-rule {
  width: 48px;
  height: 2px;
  background: #8f5238;
  margin-top: 28px;
}

.intro-text p {
  margin: 0 0 22px;
  color: #4a3028;
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
