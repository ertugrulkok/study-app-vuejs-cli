<template>
    <header>
        <h1>{{title}}</h1>
    </header>
</template>
<script>
    export default {
        props:['title']
    }
</script>

<style scoped>

header{
    width: 100%;
    min-height: 5rem;
    border-bottom: 2px solid black;
    background-color: rebeccapurple;
    color: white;
    display: flex;
    align-items: center;
    justify-content:center;
    margin:0;

}

</style>