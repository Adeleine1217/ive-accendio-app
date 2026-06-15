<template>
  <footer class="site-footer">
    <p>IVE — ACCENDIO</p>
    <p>A Nuxt practice page by Adeleine Wang · 2024</p>
  </footer>
</template>

<style scoped>
.site-footer {
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-wrap: wrap;
  gap: 12px;
  padding: 40px clamp(24px, 6vw, 80px);
  border-top: 1px solid rgba(124, 92, 77, 0.2);
  background: rgba(255, 250, 246, 0.5);
  color: #7c5c4d;
  font-size: 12px;
  letter-spacing: 0.12em;
  text-transform: uppercase;
}

.site-footer p {
  margin: 0;
}
</style>
