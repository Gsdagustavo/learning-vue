<script lang="ts" setup></script>

<template>
  <footer>
    <div class="description">
      <h1>Cachaçaria Wilbert</h1>
      <small class="copyright">© 2025 Cachaçaria Wilbert. Todos os direitos reservados.</small>
      <p>
        Tradição e qualidade na produção de cachaças artesanais, com respeito ao processo, aos
        nossos clientes e à história de Pomerode.
      </p>
    </div>

    <address class="links">
      <a aria-label="Instagram" href="https://www.instagram.com/cachacawilbertpomerode/">
        <i class="link fab fa-instagram"></i>
      </a>
      <a aria-label="Localização" href="https://maps.app.goo.gl/gQwTm5FWsEzhDuHM9">
        <i class="link fa-solid fa-map"></i>
      </a>
    </address>
  </footer>
</template>

<style scoped>
* {
  font-size: 14px;
}

footer {
  margin-top: 50px;
  background: var(--primary-color);
  text-align: center;
  display: flex;
  flex-direction: column;
  position: relative;
  bottom: 0;
  gap: 12px;
  padding: 24px;
  width: 100%;
}

h1 {
  font-size: 20px;
  margin-bottom: 12px;
}

.links {
  display: flex;
  justify-content: center;
  gap: 16px;
}

.link {
  transition:
    font-size 0.2s ease,
    color 0.2s ease;
  font-size: 36px;
}

.link:hover {
  color: var(--accent-hover);
}
</style>
