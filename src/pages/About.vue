<script lang="ts" setup>
import Card from '@/components/Card.vue'
</script>

<template class="template">
  <div class="container">
    <Card justify-content="space-between" margin-top="50px">
      <div class="description">
        <h1>Sobre nós</h1>
        <p>
          A história do nosso alambique começou há cerca de 60 anos, com meu pai, Victor Wilbert.
          Desde o início, ele se dedicava à produção de cachaças puras, prezando pela tradição e
          pela qualidade, raramente se aventurando em bebidas saborizadas. O negócio sempre foi
          familiar, sem intenção de expansão, com vendas restritas a amigos e conhecidos. Com o
          passar dos anos, após meu casamento, surgiu a oportunidade de dar continuidade a esse
          legado. Reservei um espaço em meu próprio terreno e iniciei a construção do alambique,
          movido pelo desejo de manter viva a paixão que meu pai sempre teve pela produção
          artesanal. Assim que a produção começou, percebi que a aceitação do produto na região era
          extremamente positiva. Os consumidores, em sua maioria conhecidos, demonstravam grande
          apreço pela qualidade da cachaça. Diante disso, decidi investir no crescimento do negócio.
          Hoje, além das cachaças tradicionais, produzimos diversos sabores de cachaças e licores,
          todos fermentados e armazenados em barris de carvalho, mantendo o cuidado artesanal em
          cada etapa do processo. Atualmente, nossos produtos são comercializados em municípios como
          Pomerode, Blumenau, Gaspar, Luiz Alves, entre outros, sempre com o compromisso de
          preservar a tradição, a qualidade e o sabor que marcaram o início dessa história.
        </p>
      </div>
      <div class="images">
        <img alt="Donos da cachaçaria" src="/images/owners.jpg" />
        <img alt="Interior da cachaçaria" src="/images/store.jpg" />
      </div>
    </Card>
  </div>
</template>

<style scoped>
.container {
  min-height: calc(100vh - 100px);
  display: flex;
  align-items: center;
  justify-content: center;
}

.card {
  padding: 42px;
  max-width: 60vw;
  border-radius: 8px;
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.26);
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  gap: 50px;
}

h1 {
  margin-top: 12px;
  color: rgb(78, 46, 27);
  font-weight: bold;
  font-size: 32px;
}

p {
  margin-top: 32px;
  line-height: 1.5;
  text-align: justify;
  color: rgb(102, 68, 34);
}

.images {
  display: flex;
  flex-direction: column;
  justify-content: center;
  gap: 32px;
}

img {
  width: 450px;
  border-radius: 12px;
}
</style>
