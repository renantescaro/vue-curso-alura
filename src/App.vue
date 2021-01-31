<template>
  <div>
    <h1>{{ titulo }}</h1>

    <ul>
      <li v-for="(foto, i) of fotos" :key="i">
        <img :src="foto.url" :alt="foto.titulo">
      </li>
    </ul>

  </div>
</template>

<script>
export default {
  name: 'app',
  data () {
    return {
      titulo : 'Alura Pic!',
      fotos  : [
        {
          url    : 'https://s2.glbimg.com/slaVZgTF5Nz8RWqGrHRJf0H1PMQ=/0x0:800x450/984x0/smart/filters:strip_icc()/i.s3.glbimg.com/v1/AUTH_59edd422c0c84a879bd37670ae4f538a/internal_photos/bs/2019/U/e/NTegqdSe6SoBAoQDjKZA/cachorro.jpg',
          titulo : 'Cachorro 1',
        },
        {
          url    : 'https://super.abril.com.br/wp-content/uploads/2018/05/filhotes-de-cachorro-alcanc3a7am-o-c3a1pice-de-fofura-com-8-semanas1.png',
          titulo : 'Cachorro 2',
        },
        {
          url    : 'https://conteudo.imguol.com.br/c/entretenimento/54/2020/04/28/cachorro-pug-1588098472110_v2_450x337.jpg',
          titulo : 'Cachorro 3',
        }
      ]
    }
  }
}
</script>

<style>

</style>
