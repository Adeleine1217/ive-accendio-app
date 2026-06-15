<script setup>
const members = [
  {
    name: 'Yujin',
    korean: '안유진',
    title: 'Leader Energy',
    line: 'The composed centre of gravity — bright, athletic, and quietly commanding.',
    symbol: '🐶'
  },
  {
    name: 'Gaeul',
    korean: '가을',
    title: 'Autumn Elegance',
    line: 'Calm, graceful, and precise — the kind of presence that does not need to chase attention.',
    symbol: '🍂'
  },
  {
    name: 'Rei',
    korean: '레이',
    title: 'Dreamy Rebel',
    line: 'Soft-spoken but distinctive, with a playful coolness that makes every detail memorable.',
    symbol: '🦋'
  },
  {
    name: 'Wonyoung',
    korean: '장원영',
    title: 'Iconic Muse',
    line: 'A polished star image with unbelievable control — elegant, aspirational, and instantly recognisable.',
    symbol: '🪽'
  },
  {
    name: 'Liz',
    korean: '리즈',
    title: 'Golden Voice',
    line: 'Warm, emotional, and luminous — the voice that gives the song its soft inner glow.',
    symbol: '🎙️'
  },
  {
    name: 'Leeseo',
    korean: '이서',
    title: 'Youngest Spark',
    line: 'Fresh, sharp, and fearless — the maknae energy that keeps IVE feeling alive and forward-looking.',
    symbol: '✨'
  }
]
</script>

<template>
  <section class="members-section">
    <div class="inner">
      <div class="section-intro">
        <p class="eyebrow">DIVE Notes</p>
        <h2>Six reflections of an incandescent spell</h2>
        <p>
          A small member guide written through my own fan lens — each voice
          contributes to ACCENDIO's darkly luminous atmosphere and ritual tone.
        </p>
      </div>
      <div class="members-grid">
        <MemberCard
          v-for="member in members"
          :key="member.name"
          :symbol="member.symbol"
          :korean="member.korean"
          :name="member.name"
          :title="member.title"
          :line="member.line"
        />
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

.members-section {
  padding: 96px clamp(24px, 6vw, 80px) 120px;
  background: #f0e5da;
  border-top: 1px solid rgba(124, 92, 77, 0.12);
}

.section-intro {
  max-width: 760px;
  margin-bottom: 52px;
}

.section-intro h2 {
  margin: 12px 0 24px;
  color: #241915;
  font-size: clamp(40px, 7vw, 88px);
  line-height: 0.95;
  letter-spacing: -0.06em;
}

.section-intro p {
  margin: 0;
  color: #6b4f43;
  font-size: 20px;
  line-height: 1.7;
}

.members-grid {
  display: grid;
  grid-template-columns: repeat(3, minmax(0, 1fr));
  gap: 22px;
}

@media (max-width: 960px) {
  .members-grid {
    grid-template-columns: repeat(2, minmax(0, 1fr));
  }
}

@media (max-width: 640px) {
  .members-section {
    padding: 72px 24px 96px;
  }

  .members-grid {
    grid-template-columns: 1fr;
  }
}
</style>
