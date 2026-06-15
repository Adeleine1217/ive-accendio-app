<template>
  <section class="video-section">
    <div class="inner video-inner">
      <div class="video-meta">
        <p class="eyebrow">Watch</p>
        <h2 class="video-heading">ACCENDIO<br><em>Official M/V</em></h2>
        <p class="video-desc">
          A moonlit ritual of lacquered mirrors and precise movement. The
          official music video is the visual key to the essay's darker,
          cinematic reading.
        </p>
      </div>
      <div class="video-stage">
        <div class="video-frame">
          <iframe
            src="https://www.youtube.com/embed/PGLx4V680J8"
            title="IVE (아이브) 'ACCENDIO' Official MV"
            allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
            allowfullscreen
          />
        </div>
        <p class="video-caption">IVE (아이브) ‘ACCENDIO’ Official MV</p>
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

.video-section {
  padding: 96px clamp(24px, 6vw, 80px) 112px;
  background: #12080f;
  border-top: 1px solid rgba(255, 213, 165, 0.08);
}

.video-inner {
  display: grid;
  grid-template-columns: 260px 1fr;
  gap: 72px;
  align-items: start;
}

.video-meta {
  position: sticky;
  top: 48px;
}

.video-heading {
  margin: 12px 0 28px;
  color: #f4e8d7;
  font-size: clamp(32px, 4vw, 52px);
  line-height: 1;
  letter-spacing: -0.05em;
}

.video-heading em {
  color: #d4a16e;
  font-style: italic;
}

.video-desc {
  margin: 0;
  color: #c9b3a0;
  font-size: 17px;
  line-height: 1.8;
}

.video-stage {
  display: flex;
  flex-direction: column;
  gap: 20px;
}

.video-frame {
  border-radius: 20px;
  overflow: hidden;
  border: 1px solid rgba(212, 161, 110, 0.22);
  box-shadow:
    0 0 0 6px rgba(212, 161, 110, 0.06),
    0 40px 120px rgba(0, 0, 0, 0.5);
  aspect-ratio: 16 / 9;
}

.video-frame iframe {
  display: block;
  width: 100%;
  height: 100%;
  border: 0;
}

.video-caption {
  margin: 0;
  color: #a88a75;
  font-size: 12px;
  letter-spacing: 0.14em;
  text-transform: uppercase;
  text-align: right;
}

@media (max-width: 960px) {
  .video-inner {
    grid-template-columns: 1fr;
    gap: 40px;
  }

  .video-meta {
    position: static;
  }

  .video-caption {
    text-align: left;
  }
}
</style>
