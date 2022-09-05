<template>
    <button :type="type" :class="mode">
    <slot></slot>
    </button>
    
</template>
<script>
    export default {
        props:['type', 'mode']
    }
</script>
<style scoped>
    button{
    padding: 8px 20px;
    border: none;
    background-color: rgb(246, 118, 72);
    color: wheat;
    font-size: 1rem;
    text-transform: uppercase;
    border-radius: 15px;
    cursor: pointer;
}
button:hover{
    background-color: rgb(145, 46, 10);
}
.curronBtn{
    background-color: transparent;
    color: rgb(226, 9, 226);
    border: none;
}
.currentBtn:Hover,
.curronBtn:active{
    background-color:rgba(32, 5, 241, 0.403) ;
}


</style>