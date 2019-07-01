<template>
  <section>
    <h1>Buy or Sell</h1>
    <ProdutosBuscar />
    <ProdutosLista />
  </section>
</template>

<script>
// @ is an alias to /src
import ProdutosBuscar from "@/components/ProdutosBuscar";
import ProdutosLista from "@/components/ProdutosLista";
export default {
  name: "home",
  components: { ProdutosBuscar, ProdutosLista }
};
</script>

<style scoped>
h1 {
  font-size: 2rem;
  color: #b9785f;
  margin-top: 40px;
  text-align: center;
}
</style>
