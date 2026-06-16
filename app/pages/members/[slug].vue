<script setup lang="ts">
import { useRoute, useRouter } from 'vue-router'
import members from '../../data/members'

const route = useRoute()
const router = useRouter()
const slug = String(route.params.slug || '')

const member = members.find(m => m.slug === slug)

if (!member) {
  // simple fallback: navigate to home if slug invalid
  router.replace('/')
}

const title = member
  ? `${member.name} — ACCENDIO Member Reflection | Adeleine Wang`
  : 'ACCENDIO Member | Adeleine Wang'

useSeoMeta({
  title,
  description: member
    ? `A short editorial reflection on ${member.name}'s presence in IVE's ACCENDIO.`
    : 'ACCENDIO member reflection page.'
})

function editorialFor(m: any) {
  return `${m.name} is the ${m.role.toLowerCase()} within ACCENDIO’s cinematic frame — ${m.accent.toLowerCase()}. Their presence transforms stillness into a reflective surface, where light and ritual fold together to create the project’s mirror-like atmosphere.`
}
</script>

<template>
  <section class="member-page">
    <div class="inner">
      <NuxtLink to="/" class="back-link">Back to ACCENDIO</NuxtLink>

      <div class="member-hero">
        <div class="symbol">{{ member.symbol }}</div>
        <div class="meta">
          <h1>{{ member.name }}</h1>
          <p class="korean">{{ member.korean }}</p>
          <p class="role">{{ member.role }}</p>
          <p class="title">{{ member.title }}</p>
        </div>
      </div>

      <div class="editorial">
        <p>{{ editorialFor(member) }}</p>
      </div>

      <aside class="quote-card">
        <p class="quote">“{{ member.quote }}”</p>
      </aside>

      <NuxtLink to="/" class="grid-link">Back to member grid</NuxtLink>
    </div>
  </section>
</template>

<style scoped>
.member-page {
  min-height: 100vh;
  background: linear-gradient(180deg,#1a0f14 0%, #241918 60%);
  color: #efe6dd;
  padding: 56px 24px;
}
.inner {
  max-width: 900px;
  margin: 0 auto;
}
.back-link {
  color: #d7c0a8;
  display: inline-block;
  margin-bottom: 28px;
  text-decoration: underline;
}
.member-hero {
  display: flex;
  gap: 28px;
  align-items: center;
  margin-bottom: 28px;
}
.symbol {
  font-size: 72px;
}
.meta h1 {
  margin: 0;
  font-size: 48px;
  color: #fdeedc;
}
.korean {
  margin: 6px 0 12px;
  color: #c8a686;
  letter-spacing: .12em;
}
.role, .title {
  margin: 0;
  color: #b99673;
  font-weight: 600;
  text-transform: uppercase;
  letter-spacing: .14em;
  font-size: 13px;
}
.editorial p {
  margin-top: 24px;
  line-height: 1.85;
  color: #e9dccf;
  font-size: 18px;
}
.quote-card {
  margin-top: 28px;
  padding: 20px;
  border-radius: 12px;
  background: rgba(255, 250, 242, 0.04);
  border: 1px solid rgba(217, 176, 126, 0.08);
}
.quote {
  margin: 0;
  color: #f6eadf;
  font-style: italic;
}
.grid-link {
  display: inline-block;
  margin-top: 30px;
  color: #d7c0a8;
  text-decoration: underline;
}

@media (max-width: 720px) {
  .member-hero { flex-direction: row; align-items: flex-start }
  .meta h1 { font-size: 36px }
  .symbol { font-size: 56px }
}
</style>
