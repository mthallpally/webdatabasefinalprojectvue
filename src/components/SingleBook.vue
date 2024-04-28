<template>
    

    <div  :class="book.Status ? 'green': 'red' ">

                        <h2>vent id : {{book.ventid}}</h2>
                        <h4>Hospital name:             {{book.Hospitalname}}</h4>
    
                        <h4>Address  :             {{book.Address}}</h4>
                        <h4>Contact         :             {{book.Contact  }}</h4>
                        

    </div>          
</template>

<script>

export default{
    name: 'SingleBook',
    props:{
        book: Array
    }
}
</script>

<style scoped>

.green{
    background-color: green;
}

h4{
    margin: 2px;
}

div{
    background-color: #ffb89e;
    color: black;
    padding: 1em;
    text-align: center;
    width: 80%;
    margin: auto;
    

}

.red{
background-color: orangered !important;

}


</style>