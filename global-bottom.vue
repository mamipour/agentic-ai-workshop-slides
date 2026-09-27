<template>
  <div class="intenteye-bg" aria-hidden="true">
    <div class="blob blob-blue" />
    <div class="blob blob-purple" />
    <div class="blob blob-pink" />
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
  filter: blur(90px);
  animation: pulse 8s ease-in-out infinite;
}

.blob-blue {
  width: 600px;
  height: 600px;
  top: -200px;
  left: -200px;
  background: rgba(59, 130, 246, 0.35);
  animation-delay: 0s;
}

.blob-purple {
  width: 600px;
  height: 600px;
  bottom: -200px;
  right: -200px;
  background: rgba(168, 85, 247, 0.35);
  animation-delay: 2.5s;
}

.blob-pink {
  width: 400px;
  height: 400px;
  top: 40%;
  left: 45%;
  transform: translate(-50%, -50%);
  background: rgba(236, 72, 153, 0.2);
  animation-delay: 5s;
}

@keyframes pulse {
  0%, 100% { opacity: 1; transform: scale(1); }
  50% { opacity: 0.75; transform: scale(1.1); }
}
</style>
