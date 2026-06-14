<template>
  <section class="video-section">
    <div class="inner video-inner">
      <div class="video-meta">
        <p class="eyebrow">Watch</p>
        <h2 class="video-heading">REBEL HEART<br><em>Official M/V</em></h2>
        <p class="video-desc">
          Six members. One defiant heartbeat. Watch the official music video
          and feel exactly what this essay is trying to describe.
        </p>
      </div>
      <div class="video-stage">
        <div class="video-frame">
          <iframe
            src="https://www.youtube.com/embed/g36q0ZLvygQ"
            title="IVE (아이브) 'REBEL HEART' Official MV"
            allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
            allowfullscreen
          />
        </div>
        <p class="video-caption">IVE (아이브) &lsquo;REBEL HEART&rsquo; Official MV</p>
      </div>
    </div>
  </section>
</template>

<style scoped>
.eyebrow {
  margin: 0 0 20px;
  color: #c8906a;
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
  background: #2a1a13;
  border-top: 1px solid rgba(0, 0, 0, 0.18);
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
  color: #f5e8de;
  font-size: clamp(32px, 4vw, 52px);
  line-height: 1;
  letter-spacing: -0.05em;
}

.video-heading em {
  color: #c8906a;
  font-style: italic;
}

.video-desc {
  margin: 0;
  color: #b09080;
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
  border: 1px solid rgba(200, 144, 106, 0.22);
  box-shadow:
    0 0 0 6px rgba(200, 144, 106, 0.06),
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
  color: #6b4a38;
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
