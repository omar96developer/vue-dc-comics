<template>
    <header>
        <nav>
            <div class="nav_container">
                <div class="nav_logo">
                    <img src="../assets/img/dc-logo.png" alt="dc-logo">
                </div>
                <div class="nav_items">
                    <ul class="nav_items_list">
                        <li class="nav_item" 
                        v-for="(item, i) in navbarItems" :key="i"
                        :class="i === currentActive ? 'active' : '' ">
                            <a :href="item.href">{{item.title}}</a>
                        </li>
                    </ul>
                </div>
            </div>
        </nav>

    </header>
</template>
<script>
export default {
    name: "Header",
    data(){
        return {
            navbarItems: [
                {
                    title: 'CHARACTERS',
                    href: '#'
                },
                {
                    title: 'COMICS',
                    href: '#'
                },
                {
                    title: 'MOVIES',
                    href: '#'
                },
                {
                    title: 'TV',
                    href: '#'
                },
                {
                    title: 'GAMES',
                    href: '#'
                },
                {
                    title: 'COLLECTIONS',
                    href: '#'
                },
                {
                    title: 'VIDEOS',
                    href: '#'
                },
                {
                    title: 'FANS',
                    href: '#'
                },
                {
                    title: 'NEWS',
                    href: '#'
                },
                {
                    title: 'SHOP',
                    href: '#'
                }
                
            ],
            currentActive: 0,
        }
    }
    
}

</script>
