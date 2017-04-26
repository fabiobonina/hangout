<template>
    <div>
        <h1>Aqui é o modulo de vendas</h1>
        <a href="#" @click="mudarSentenca">Click aqui!</a>
    </div>
</template>

<script>
 export default {
     methods: {
         mudarSentenca () {
             this.dispatch('mudar-sentenca', { sentenca: 'Novo texto a ser exibido TobBar!' })
         },
     },
 }
</script>