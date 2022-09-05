<template>
  
    <li>
      <base-card>
        <header>
            <h3>{{ titleP}}</h3>
            <base-button mode="currentBtn">Delete</Base-button>
        </header>
      
        <p>{{ descriptionP }}</p>
        <nav>
            <a :href="linkP">View Learning Platform</a>
        </nav>
        </base-card>
    </li>
</template>
<script>

    export default{
        props:["titleP", "descriptionP","linkP"],
        components:{
          
        } 
    }
</script>
<style scoped>
li{
    margin: auto;
    max-width: 500px;
    list-style: none;
    text-align: left;
    }
header{
    display: flex;
    justify-content: space-between;
    align-items: center;
}

a:hover{
    color:rgb(234, 150, 119); 
}

</style>