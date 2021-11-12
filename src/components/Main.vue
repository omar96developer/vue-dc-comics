<template>
    <main>
        <section class="main_section1">
            <div class="container_section1">
                <h2>{{title}}</h2>
            </div>
        </section>
        <section class="main_section2">
            <div class="container_section2">
                 <ul class="list_items">
                   <li class="list_item" 
                    v-for="(item, i) in mainItems" :key="i">
                        <img :src="require(`../assets/img/${item.img}`)" alt="#">                   
                        <a href="#">{{item.title}}</a>
                    </li>
                </ul>
            </div>
        </section>
    </main>
</template>
<script>
export default {
    name: "main",
    data(){
        return {
            title:'-->Content goes here<--',
             mainItems: [
                {
                    img:'buy-comics-digital-comics.png',
                    title: 'DIGITAL COMICS',  
                },
                {
                    img:'buy-comics-merchandise.png',
                    title: 'DC MERCHANDISE',
                },
                {
                    img:'buy-comics-subscriptions.png',
                    title: 'SUBSCRIPTION',
                },
                {
                    img:'buy-comics-shop-locator.png',
                    title: 'COMIC SHOP LOCATOR', 
                },
                {
                    img:'buy-dc-power-visa.svg',
                    title: 'DC POWER VISA', 
                }
            ],
            

        }
    }
    
}

</script>
