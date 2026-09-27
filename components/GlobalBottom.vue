<template>
  <div class="intenteye-bg" aria-hidden="true">
    <div class="blob blob-blue" />
    <div class="blob blob-purple" />
    <div class="blob blob-pink" />
    <div class="noise-overlay" />
  </div>
</template>

<style scoped>
.intenteye-bg {
  position: fixed;
  inset: 0;
  z-index: 0;
  background: linear-gradient(135deg, #030712 0%, #0f172a 40%, #111827 70%, #000000 100%);
  overflow: hidden;
  pointer-events: none;
}

.blob {
  position: absolute;
  border-radius: 50%;
  filter: blur(80px);
  animation: pulse 8s ease-in-out infinite;
}

.blob-blue {
  width: 500px;
  height: 500px;
  top: -150px;
  left: -150px;
  background: rgba(59, 130, 246, 0.22);
  animation-delay: 0s;
}

.blob-purple {
  width: 500px;
  height: 500px;
  bottom: -150px;
  right: -150px;
  background: rgba(168, 85, 247, 0.22);
  animation-delay: 2.5s;
}

.blob-pink {
  width: 350px;
  height: 350px;
  top: 40%;
  left: 45%;
  transform: translate(-50%, -50%);
  background: rgba(236, 72, 153, 0.12);
  animation-delay: 5s;
}

.noise-overlay {
  position: absolute;
  inset: 0;
  background-image: url("data:image/svg+xml,%3Csvg viewBox='0 0 256 256' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='noise'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.9' numOctaves='4' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23noise)' opacity='0.03'/%3E%3C/svg%3E");
  background-repeat: repeat;
  background-size: 200px 200px;
  opacity: 0.4;
}

@keyframes pulse {
  0%, 100% { opacity: 1; transform: scale(1); }
  50% { opacity: 0.7; transform: scale(1.08); }
}
</style>
