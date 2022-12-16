<template>
  <p>Sem a diretiva</p>
  <!-- <p v-texto="{ cor: 'red', tamanhoFonte: '200%', totalCaracteres: 15 }">Minha primeira diretiva customizada</p>
  <p v-texto="configuracaoTexto">Teste</p> -->
  <div v-posicao:absolute="75" v-texto="{ cor: 'green', totalCaracteres: 100 }">Olá, eu sou um binding de argumento e valor</div>
  <span>Código A: </span><input type="text"><span v-informacao:destacado.umClickMouse.sairAutomaticamente="'Você encontrará o código A na parte frontal do equipamento.'"> i</span>
  <p v-colorir>Texto colorido</p>
</template>

<script>
import colorirFundoTexto from '@/directives/colorirFundoTexto';

export default {
  name: 'App',
  directives: {
    colorir: colorirFundoTexto
  },
  data: () => ({
    configuracaoTexto: { cor: 'blue', tamanhoFonte: '300%', totalCaracteres: 4 }
  })
}
</script>

<style>
</style>
