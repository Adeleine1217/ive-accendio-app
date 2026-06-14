<script setup>
defineProps({
  symbol: String,
  korean: String,
  name: String,
  title: String,
  line: String
})
</script>

<template>
  <article class="member-card">
    <div class="member-symbol">{{ symbol }}</div>
    <p class="member-korean">{{ korean }}</p>
    <h3>{{ name }}</h3>
    <p class="member-title">{{ title }}</p>
    <p class="member-line">{{ line }}</p>
  </article>
</template>

<style scoped>
.member-card {
  min-height: 320px;
  padding: 36px;
  border: 1px solid rgba(124, 92, 77, 0.18);
  border-radius: 28px;
  background:
    linear-gradient(145deg, rgba(255, 255, 255, 0.74), rgba(255, 246, 240, 0.44)),
    rgba(255, 255, 255, 0.38);
  box-shadow: 0 20px 60px rgba(63, 39, 29, 0.06);
  transition:
    transform 0.28s ease,
    box-shadow 0.28s ease;
}

.member-card:hover {
  transform: translateY(-8px);
  box-shadow: 0 32px 90px rgba(63, 39, 29, 0.13);
}

.member-symbol {
  margin-bottom: 28px;
  font-size: 42px;
}

.member-korean {
  margin: 0 0 8px;
  color: #a06f52;
  font-size: 14px;
  letter-spacing: 0.14em;
}

h3 {
  margin: 0;
  color: #241915;
  font-size: 42px;
  line-height: 1;
  letter-spacing: -0.05em;
}

.member-title {
  margin: 14px 0 20px;
  color: #8f5238;
  font-size: 13px;
  font-weight: 700;
  letter-spacing: 0.16em;
  text-transform: uppercase;
}

.member-line {
  margin: 0;
  color: #5d453c;
  font-size: 17px;
  line-height: 1.75;
}

@media (max-width: 640px) {
  .member-card {
    min-height: auto;
  }
}
</style>
