<template>
    <div class="top-bar">
        <h1>Seja bem vindo ao 1° aula </h1>
        <p>{{ message }}</p>
    </div>
</template>

<script>
    export default {
        data() {
            return {
                message: 'Aqui posso colocar um conteudo qualquer!'
            }
        }
    }
</script>


<style scoped>
    .top-bar{
        position: fixed;
        top: 0;
        left: 0;
        right: 0;
        padding: 5px;
        backgroud-color: #ccc;
    }
</style>