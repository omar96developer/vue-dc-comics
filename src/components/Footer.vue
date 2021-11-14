<template>
    <footer>
        <div class="footer_container_1">
            <div class="footer_container_A">
                <section class="footer1">

                    <div class="footer1_list">
                        <div class="list">

                            <h3>DC COMICS</h3>
                            <ul>
                                <li v-for="(value, i) in dccomic" :key="i">{{value}}</li>                                
                            </ul>

                            <h3>SHOP</h3>
                            <ul>
                                <li v-for="(value, i) in shop" :key="i">{{value}}</li>                                
                            </ul>
                        </div>
                        <div class="list">
                            <h3>DC</h3>
                            <ul>
                                <li v-for="(value, i) in dc" :key="i">{{value}}</li>                               
                            </ul>
                        </div>
                        <div class="list">
                            <h3>SITES</h3>
                            <ul>
                                <li v-for="(value, i) in sites" :key="i">{{value}}</li>
                            </ul>
                        </div>
                    </div>

                    <div class="footer1_img">
                        <div class="footer_logo">
                            <img src="@/assets/img/dc-logo-bg.png" alt="#">
                        </div>
                        
                    </div>
                </section>
            </div>
        </div>
        <div class="footer_container_2">
            <div class="footer_container_B">
                <section class="footer2">
                    <div class="signup">
                        <a href="#">
                            SIGN-UP NOW!
                        </a>
                    </div>
                    <div class="follow">
                        <h3>FOLLOW US</h3>
                        <img src="@/assets/img/footer-facebook.png" alt="#">
                        <img src="@/assets/img/footer-twitter.png" alt="#">
                        <img src="@/assets/img/footer-youtube.png" alt="#">
                        <img src="@/assets/img/footer-pinterest.png" alt="#">
                        <img src="@/assets/img/footer-periscope.png" alt="#">

                    </div>
                </section>
            </div>
        </div>
       
    </footer>
</template>
<script>
export default {
    name: "Footer",
    data(){
        return {
           dccomic: {
                li1: 'Characters',
                li2: 'Comics',
                li3: 'Movies',
                li4: 'TV',
                li5: 'Games',
                li6: 'Videos',
                li7: 'News'
           },
           shop: {
                li1: 'Shop DC',
                li2: 'Shop DC Collectables'
           },
           dc: {
                li1: 'Terms Of Use',
                li2: 'Privacy policy (New)',
                li3: 'Ad Choices',
                li4: 'Advertsing',
                li5: 'Jobs',
                li6: 'Subscriptions',
                li7: 'Talent Workshops',
                li8: 'CPRSC Certificates',
                li9: 'li1:Rating',
                li10: 'Shop Help',
                li111: 'Contact Us'
           },
           sites:{
                li1: 'DC',
                li2: 'MAD Magazine',
                li3: 'DC Kids',
                li4: 'DC Universe',
                li5: 'DC Power Visa'
           }
        }
    }
    
}

</script>
