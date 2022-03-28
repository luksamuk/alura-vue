<template>
<div>
  <h1>{{ titulo }}</h1>
  <ul>
    <li v-for="(foto, index) of fotos" :key="index">
      <img :src="foto.url" :alt="foto.titulo">
    </li>
  </ul>
</div>
</template>

<script>
export default {
    data: () => {
	return {
	    titulo: 'Alurapic',
	    fotos: [
		{
		    url: 'https://i.ytimg.com/vi/8qA4UOLnC5A/maxresdefault.jpg',
		    titulo: 'cachorro'
		},
		{
		    url: 'https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fpubimg.band.uol.com.br%2Ffiles%2F31f64ead7787bbfededd.png&f=1&nofb=1',
		    titulo: 'Cachorrão'
		}
	    ]
	}
    }
}
</script>

<style>

</style>
