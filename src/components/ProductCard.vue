<template>
    <div class="product_card" >
        <img :src="immagine" alt="#">
        <h4>{{titolo}}</h4>
        <div class="overlay">
            <p>Prezzo: {{prezzo}}</p>
            <p>Tipo: {{tipo}}</p>
        </div>
        
    </div>  
</template>

<script>
export default {
    name: 'ProductCard',
    props:['immagine', 'titolo', 'prezzo', 'tipo']
}    
</script>