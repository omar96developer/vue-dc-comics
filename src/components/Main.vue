<template>
    <main>
        <section class="main_section1">
            <div class="container_section1">
                <h2>{{title}}</h2>
            </div>
        </section>
        <section class="main_section2">
            <div class="container_section2">
                 <ul class="list_item">
                    <li class="nav_item" 
                    v-for="(item, i) in mainItems" :key="i">
                        <img src="../assets/img/buy-comics-digital-comics.png" alt="#">                   
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
                    title: 'DC MERCHANDISE',
                   
                },
                {
                    title: 'SUBSCRIPTION',
                    
                },
                {
                    title: 'COMIC SHOP LOCATOR',
                    
                },
                {
                    title: 'DC POWER VISA',
                    
                }
            ],
            

        }
    }
    
}

</script>
