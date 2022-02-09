<template>
    <footer class="blue-gradient">
        <div class="ft-top">
            <div class="ft-top-box"> 
                <div class="logo">
                    <img src="@/assets/images/white-logo-2.png" alt="">
                </div>
                <p>When, while the lovely valley teems vapour around meand meridian sun strikes the upper impenetrable</p>
            </div>

            <div class="ft-top-box links"> 
                <h3>Quick Links</h3>
                <ul v-for="(link, i) in links" :key="i" :link="link">
                    <li>{{link}}</li>
                </ul>
            </div>

            <div class="ft-top-box resources"> 
                <h3>Resources</h3>
                <ul v-for="(resource, i) in resources" :key="i" :resource="resource">
                    <li>{{resource}}</li>
                </ul>
            </div>

            <div class="ft-top-box contacts">
                <h3>Contacts Us</h3>
                <div v-for="(contact, i) in contacts" :key="i" :contact="contact">
                    <span class="contact-type"><b>{{contact.type}}</b>:</span> 
                    <span class="contact-value">{{contact.value}}</span>
                </div>
            </div>
        </div>

        <hr>

        <div class="ft-bottom">
            <div class="copyright">
                © 2020 Phlox. All Rights Reserved.
            </div>

            <!-- <div class="social"> 
                <font-awesome-icon icon="fa-brands fa-instagram" />
                <div class="linkedin"></div>
                <div class="facebook"></div>
                <div class="twitter"></div>

                <div class="arrow-top"></div>
                <div class="chat"></div>
            </div> -->

        </div>
    </footer>
</template>

<script>
export default {
    name: 'Footer',
    props: {
        links: Array,
        resources: Array,
        contacts: Array,
    }
}
</script>

<style lang="scss" scoped>
@import '@/style/footer.scss';
@import url('https://use.fontawesome.com/releases/v5.7.1/css/all.css');

</style>